---
layout: splash
author_profile: true
class: wide
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
    title: "<h4>Micro Service Architecture</h4>"
    excerpt: ".Python, FastAPI, SQLAlchemy <br>
              .k8s, docker-compose <br> 
              .Redis, Kafka."
  - alt: "placeholder image 2"
    title: "<h4>Data engineering</h4>"
    excerpt: ".Pandas, Tensorflow Serving<br>
              .MinIO, Airflow, ELK, Grafana<br>
              .사내 Data Science - Advanced"
  - alt: "DB"
    title: "<h4>DB</h4>"
    excerpt: ".mongoDB<br>
              .ElasticSearch<br>
              .SQL(oracle, mssql)"
  - alt: "etc"
    title: "<h4>etc</h4>"
    excerpt: ".linux<br>
              .jira, confluence, bitbucket<br>
              .spotfire"
feature_row2:
  - image_path: /assets/images/cakd.JPG
    alt: "placeholder image 2"
    title: "<h4>k8s 개발/테스트환경구축</h4>"
    excerpt: '폐쇄망내 alpine기반 사내개발package build된 docker image빌드<br>  
              [k8s 로컬개발환경 구축](https://sjw451.github.io/sw/vagrant_k8s/)<br>
              Certified kubernetes administer (22.1)'

feature_row3:
  - image_path: /assets/images/airflow_logo.png
    alt: "Airflow 개발/운영"
    title: "<h4>데이터 workflow 개발/운영</h4>"
    excerpt: '-제조설비데이터 workflow 인 Apache Airflow 개발/운영<br>  
              -설비로그 데이터가공/분석 dag 개발<br>
              -kafka, redis, s3, http, grpc, elasticsearch, mongodb 등 IF위한 connection/hook개발<br>
              -k8s상 안정적 데이터 처리위해 airflow cofig 및 각종 param 검증/tunning<br>
              -airflow 부하테스터(rest api), connection 복구 script'

feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image2"
    title: "<h4>생산스케줄러 실시간 테스트 비교분석 개발</h4>" 
    excerpt: '-실시간 데이터 스케줄링 테스트/비교분석<br>
              -python, pandas pivot, openpyxl, bs3 등 활용 데이터 파싱가공<br>
              -asyncio,subprocess등 멀티프로세싱사용한 동시테스트<br>
              -실시간 운영 데이터수집(csv,xml 등)하여 0.01초대 오차'
feature_row5:
  - image_path: /assets/images/fastapi_logo.png
    alt: "placeholder image3"
    title: "<h4>팀 workdiary 데이터 api 개발</h4>"
    excerpt: '-팀 800여명이 매일 작성하는 Confluence workdiary<br>
              -부서간 협업강화를 위해 html 크롤링 및 API를 통한 제공(json)<br>
              -confluence 내 키워드 검색 제공'
---

{% include feature_row id="intro" type="center" %}

@role
- k8s 기반 데이터 파이프라인 서비스 개발/운영 
- 설비로그 관련  데이터엔지니어링
- MLOps에 관심이 있습니다. 
- ## 삼성전자 DS부문 SW Engineer(2016~)
- Samsung SW Certificate 'Professional'
- DS Data Science(DS2) 'Advanced'
<br>
<br>
<br>

@skill  

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="left" %}

{% include feature_row id="feature_row5" type="right" %}

<!-- "<h4><a href="https://sjw451.github.io/sw/replay-test/"> 생산스케줄러 실시간 테스트 비교분석 개발 </a></h4>" -->