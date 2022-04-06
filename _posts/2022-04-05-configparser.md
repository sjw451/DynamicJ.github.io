---
title:  "configparser"
header:
  teaser: "/assets/images/500x300.png"
categories: 
  - sw
tags:
  - python
  - test
  - replaytest
  - configparser
---

configuration파일 reader   
json보다 가독성이 좋음.   
개발자아닌사람이 세팅하기에 부담이 없음.   

ex)
config파일
```
[info]
rulename=Run_QTS_LSI
rev_num=11111
targetserver=mss07s
oldport=7293
newport=8293
server_interval=60
input_interval=60
test_cnt=1
[@atr1_old]
1=$SEND_USER:ONE_LINE,$RUNNING_EQPTYPE:EPOLOX
[@atr2_old]
1=$SEND_USER:ONE_LINE,$RUNNING_EQPTYPE:EPOLOX

```

propertyreader
```python
def getProperties(filename:str):
    
    dic:Dict[str,Dict[str,list]]={}
    config=confparser(filename)
    #...생략...
```   
   
   
   
   
<!-- 다른 글
<hr/>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul> -->