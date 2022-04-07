---
layout: splash
author_profile: true
# header:
#   overlay_color: "#000"
#   overlay_filter: "0.5"
#   overlay_image: /assets/images/unsplash-image-1.jpg
#   actions:
#     - label: "Download"
#       url: "https://github.com/mmistakes/minimal-mistakes/"
#   caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
# excerpt: ""안녕하세요.<br> 
#               저는 배우기를 좋아하고 열정적으로 일하고 싶어하는 개발자입니다.<br>   
#               능동적으로 일하는 것을 좋아합니다"."
intro: 
  - excerpt: "안녕하세요.<br> 
              저는 배우기를 좋아하고 열정적으로 일하고 싶어하는 개발자입니다.<br>   
              능동적으로 일하는 것을 좋아합니다"
feature_row:
  - alt: "placeholder image 1"
    title: "Micro Service Architecture"
    excerpt: ".Python, FastAPI, SQLAlchemy <br>
              .k8s, docker-compose <br> 
              .Redis, Kafka."
  - alt: "placeholder image 2"
    title: "Data engineering"
    excerpt: ".Pandas, Tensorflow Serving<br>
              .MinIO, Airflow, ELK, Grafana<br>
              .사내 Data Science - Advanced"
  - alt: "DB"
    title: "DB"
    excerpt: ".mongoDB<br>
              .ElasticSearch<br>
              .SQL(oracle, mssql)"
  - alt: "etc"
    title: "etc"
    excerpt: ".linux<br>
              .jira, confluence, bitbucket<br>
              .spotfire"
feature_row2:
  - image_path: /assets/images/cakd.JPG
    alt: "placeholder image 2"
    title: "k8s 개발환경구축 / 사내 offline환경 이미지 빌드/배포"
    excerpt: '-alpine기반 사내개발package build된 이미지배포<br>  
              -[k8s 로컬개발환경 구축](https://sjw451.github.io/sw/vagrant_k8s/)<br>
              -CKAD 자격증 취득(22년 1월)'

feature_row3:
  - image_path: /assets/images/airflow_logo.png
    alt: "데이터 workflow 개발/운영"
    title: "데이터 workflow 개발/운영"
    excerpt: '-제조설비데이터 workflow 인 Apache Airflow 개발/운영<br>  
              -Airflow Connector, Plugin, Hook 등 활용하여 데이터가공/분석 dag 개발<br>
              -k8s상 안정적 데이터 처리위해 airflow cofig 및 각종 param 검증/tunning'

feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "생산스케줄러 실시간 테스트 비교분석 개발"
    excerpt: '-실시간 데이터 스케줄러- 운영/개발 버전 테스트/비교분석
              -python, pandas pivot, openpyxl, bs3 등 활용 데이터 파싱가공'
              -asyncio,subprocess등 멀티프로세싱사용한 동시테스트
              -실시간 운영 데이터수집(csv,xml 등)하여 0.01초대 오차'
feature_row5:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image3"
    title: "팀 workdiary 데이터 api 개발"
    excerpt: '-팀 800여명이 매일 작성하는 Confluence workdiary
              -부서간 협업강화를 위해 html 크롤링 및 API를 통한 제공'
              -사람
              -실시간 운영 데이터수집(csv,xml 등)하여 0.01초대 오차'
---

{% include feature_row id="intro" type="center" %}


@MAIN JOB:
- k8s 기반 데이터 파이프라인 서비스 개발/운영 
- 설비로그 관련  데이터엔지니어링
- MLOps에 관심이 있습니다.
<br>
<br>
<br>
<br>  
@SKILL:
{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}