---
title:  "airflow 셋업"
header:
  teaser: "/assets/images/500x300.png"
categories: 
  - sw
tags:
  - kubernetes
  - k8s
  - vagrant
toc: true
toc_sticky: true
toc_label: "contents"
---


bitnami airflow helmchart 셋업(k8s)
=================================================

bitnami?
-------

가상 어플라이언스 및 웹 app, 개발 스택용 소프트웨어 패키지
공급업체/라이브러리

많이 쓰이는 아파치, nosql/sql db, airflow ,kafka등의 
통합 설치 패키지를 이미지/헬름차트로 제공
주기적 업데이트로 유지보수가 잘되고있음


airflow 셋업시 고민사항
---
- 여러대의 베어메탈 노드위에 구성된 k8s에서 운영할 버전필요
  - traffic에 능동적인 대응이 가능한지? 
  - 특정 airflow worker 다운시 distributed queue방식의 failover가 되는지? k8s
- 운영을 위한 인력이 충분한가? helmchart방식사용 
- 주기적인 업데이트가 가능한지? bitnami사제품사용

위와같은이유로 bitnami사의 airflow세가지 방식중(docker, docker-compose, helm chart)
helmchart방식으로 사용


airflow helmchart 
---
셋업을 위한 [values.yaml]({% post_url https://github.com/bitnami/charts/tree/master/bitnami/airflow %}) 설정필요하다.
airflow helmchart에는
다양한 service, configmap, deployment,statefulset 등 구성요소

그중 몇가지를 보면

- airflow
  - airflow 자체 환경변수설정
  - airflow에 추가할 패지키리스트
  - airflow deployment구성을 위한 설정
  - metric수집시 추가 설정
  - cpu/mem 할당
  - 각 deployment별 replica개수 등

- postgresql
  - externalDatabase사용여부
  - storage class 설정
- redis
  - external redis사용여부
- git repository(gitea)
  - git레포지토리
  - airflow dag/plugin git 관리여부


이러한 valus.yaml설정을 마치면 셋업자체는 간단.
helm명령어로 셋업










