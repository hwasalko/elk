# ELK Stack (Elasticsearch + Logstash + Kibana + Beats) 
> ELK Stack이란?
- Elasticsearch, Logstash, Kibana, Beats 를 일컬어 ELK Stack이라 부름
- 데이터를 수집 및 가공한 후 실시간으로 검색, 분석, 시각화 가능
- 공식 홈페이지 : https://elastic.co/kr/ 
- 한국 커뮤니티 : https://www.facebook.com/groups/elasticsearch.kr/ (facebook 그룹)
![ELK Stack](https://miro.medium.com/max/3064/0*VPlFPpkbPY15EWte.png)

* * *
   
## 1. Elasticsearch(엘라스틱서치)
> Elasticsearch란? 
- 일래스틱서치(Elasticsearch)는 루씬 기반의 분산형 검색엔진 (Apache Solr도 루씬 기반의 검색엔진)
- RESTful API 지원
- 자바로 개발되어 있으며 아파치 라이선스 조항에 의거하여 오픈 소스로 출시
- 공식 클라이언트들은 자바, 닷넷(C#), PHP, 파이썬, 그루비 등 수많은 언어로 이용이 가능
- 2020년 1월 현재 최신버전은 7.5
- AWS(아마존 클라우드), GCP(구글 클라우드)에서 클라우드 서비스 형태로도 이용 가능
- 라이센스는 다음과 같이 2 가지로 분류
    - [Apache 2.0 License] : 검색엔진 등 주요 기능 사용/수정/재배포 모두 무료로 사용 가능(상업적 이용 포함)   
    - [Elastic License] : 일부 유료기능을 제외한 모두 무료로 사용 가능(단, 사용만 무료이며 소스수정 및 재배포 불가)
    
> 주요 고객사
- 국내 : 삼성, 11번가, 네이버, 포스코 등
- 해외 : 깃허브, 아마존, 어도비, 페이스북, 넷플릭스, 이베이, 마이크로소프트, 폭스바겐, 블리자드, IBM 등


## 2. Logstash(로그스테시)
> Logstash란? 
- JRuby(jvm 기반)로 개발된 데이터 집계, 변환, 저장 도구
- Input - Filter - Output 구조로 되어 있으며 특히 'Filter'를 이용하여 다양하게 데이터 가공 가능   
(ex) IP주소 추출, 포맷변경, replace, remove 등...

## 3. Kibana(키바나)
> Kibana란?
- Elasticsearch 데이터를 시각화 할 수 있는 도구
- 다양한 차트 및 데시보드 구성을 통해 사용자에게 insight를 제시한다.
- dash board 데모 : https://demo.elastic.co/

```
 String a = 1;
 Sting b = 2;
```


## 4. Filebeat(파일비트)
- Go language로 개발된 경량 데이터 shipper
