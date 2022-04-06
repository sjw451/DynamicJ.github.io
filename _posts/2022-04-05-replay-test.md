---
title:  "Replay Test"
header:
  teaser: "/assets/images/500x300.png"
categories: 
  - sw
tags:
  - python
  - test
  - replaytest
  - portfolio
toc: true
toc_sticky: true
toc_label: "contents"
---


실시간 생산 스케줄링 시스템 테스트
=================================================

특징
----------
  - 실시간 production 환경 반영
  - data input : 
    - DB read, csv(ftp), global parameter, parameter 등...
  - data output : 
    - db wr, csv
  - 부모/자식룰의 dependency 파일 동기화
  - 운영 룰/개발 룰 동시 실행(시점차이 5분~10분 ->0.001초대로 줄임.)
  - 서버별, 회차별 다른 파라미터로 자동 구동/비교/report


<!-- Architecture
-------------
![replay test](/assets/replay_test.jpg) -->



기술
------------
- common: 
  - PropertyReader:
    - 설명: 
      - 동기화 대상 target server 기준정보 parsing
      - 스케줄링 구동 parameter parsing
      - 환경설정 read parsing
    - 사용 오픈소스: [configparser(python)]({% post_url 2022-04-05-configparser %})


  - ftpTreeManager
    - 설명: 
      - 타깃시스템-테스트서버간 실시간 파일/디렉토리 동기화
      - 특정 폴더/파일 추가/제외 (regex)
      - ex) "/test_*/readfile_*.txt"  -> 와일드카드반영하여 파일시스템동기화   
      - 해당 레벨 디렉토리 모두 조회 -> regex pattern matching시 동기화 ->최종 레벨에서 파일동기화(패턴매칭)

    - 사용 오픈소스: ftplib, re
  

  - xmlparser
    - 설명:
      - 스케줄러 및 자식 스케줄러 로직의 input parameter, 자식룰이름, sql query정보, input file정보를 담은 xml파일을 파싱
      - recursive logic
    - 사용 오픈소스: lxml(python)


  - runner
    - 설명:
      - 동시에 두개 로직 구동(개발/production)
      - 스케줄러 API 사용(subprocess)
    - 사용 오픈소스: subprocess, asyncio


  - result parser
    - 설명:
      - output csv파일 파싱
      - 부모/자식스케줄러 별 tree 구조로 데이터 sheet 정리/link
      - production/테스트 결과 비교/highlight
    - 사용 오픈소스: pandas, openpyxl, 
   

   
<!-- 다른 글
<hr/>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul> -->