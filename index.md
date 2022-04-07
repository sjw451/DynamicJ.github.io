---
layout: home
author_profile: true
# header:
#   overlay_color: "#000"
#   overlay_filter: "0.5"
#   overlay_image: /assets/images/unsplash-image-1.jpg
#   actions:
#     - label: "Download"
#       url: "https://github.com/mmistakes/minimal-mistakes/"
#   caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
# excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
intro: 
  - excerpt: "안녕하세요.<br> 
              저는 배우기를 좋아하고 열정적으로 일하고 싶어하는 개발자입니다.<br>   
              능동적으로 일하는 것을 좋아합니다"
feature_row:
  - alt: "placeholder image 1"
    title: "Micro Service Architecture"
    excerpt: ".Python, FastAPI, SQLAlchemy <br>
              .k8s, docker-compose <- CKAD <br> 
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
  - alt: "placeholder image 2"
    title: "k8s 개발환경구축 / 사내 offline환경 이미지 빌드/배포"
    excerpt: "- alpine기반 사내개발package build된 이미지배포<br>
              - k8s 로컬개발환경 구축(vagrant, virtual box, 각종 helmchart 배포)<br>
              - CKAD 자격증 취득(22년 1월)"

feature_row3:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'

feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
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