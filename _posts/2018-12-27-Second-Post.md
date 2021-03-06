# StartCamp 2주차
크롤링과 Git에 대하여

---

# [Day1] 크롤링 기초

## 크롤링에 대한 이해
* BeautifulSoup : 데이터를 가져올 사이트의 html을 가져와 원하는 데이터만 얻을 수 있다.
* Selenium : 웹앱 테스트 프레임워크로, 사용자가 원하는 페이지를 직접 띄워 원하는 html을 가져온다.

## 다양한 크롤링 기법
* Pagination : 페이지 번호가 들어가는 url을 크롤링할 때, for를 사용해 수월하게 할 수 있다.
* href : html에 있는 링크를 받아올 수 있는 태그로, 해당 태그에 들어가 html을 받아올 수 있다.
* Pagination과 href를 사용하면, 언론사의 기사 내용을 수월하게 크롤링 할 수 있다.

## 데이터 시각화
* Matplotlib : 모은 데이터로 차트를 만들 수 있다.

---

# [Day2] 데이터 분석

## 트럼프 대통령 트윗으로 시작하는 데이터 처리
* open('파일명'), read(), close() 로 파일을 열고, 읽고, 닫을 수 있다.
* word.startswith('s') : word가 's'로 시작하는 지 알 수 있다.

## 영어 단어 모음으로 시작하는 텍스트 파일 분석
* sorted() : 리스트를 특정 기준에 맞춰 정렬하는 함수

## 넷플릭스 시청 데이터로 알아보는 데이터형 변환
* dictionary : key와 item으로 이루어진 데이터 타입. key로 item을 찾을 수 있다.
   * { key1:item1, key2:item2, ... }
* set : 집합형태로 나타내어지는 데이터 타입.
   * set([1, 2, 3, 3]) = {1, 2, 3}
* json : 웹에서 정보를 나타내는데 많이 사용하는 형식으로, dictionary와 비슷함

## 테드 강연으로 다뤄보는 복잡한 형태의 데이터
* lambda : 함수를 한줄로 사용가능하게 하는 것. lambad x : x+3
* map : 특정 함수를 리스트에 적용하게 하는 것. [func(x) for x in data] -> map(func, data)

---

# [Day3] 챗봇 시작하기

## Flask 기초
* Flask : 자유도가 높고, 가볍고 심플한 웹 프레임워크 이다.
* @app.route(/) : () 안의 url일 경우, 해당 함수가 동작한다.
    * @app.route(/)
    * def hello_world():
    
## Slack Bot 소개
* 슬랙이라는 채팅 프로그램에 존재하는 슬랙 봇을 활용하여, 사용자와 대화를 하며 상호작용할 수 있게 한다.

# [Day4] 챗봇 프로젝트

## 슬랙 챗봇 프로젝트
* python, flask를 설치한 후, pycharm 코드에디터를 설치한 후, 슬랙 봇의 가이드라인에 따라
    슬랙 봇을 설정했다.

## DialogFlow 연동하기
* DialogFlow를 사용하여, 어떤 문장을 입력했을 때, 정해진 단어를 뽑아내는 플로우를 만들었다.
* 그 단어를 사용하여, 슬랙 봇과 DialogFlow을 연동했다.

## 최종 제출
* 슬랙 챗봇과 DialogFlow를 이용해, 사용자가 원하는 정보를 입력하면, 그에 맞는 정보를 크롤링해와서 대답해주는 슬랙 챗봇을 만들었다.

---

# [Day5] Git과 Git 버전 관리

## Git이란?
* 오픈소스 : 소스 코드를 공개하여, 누구나 그 코드를 보고, 사용하고, 수정하고 배포할 수 있는 소프트웨어
* Git : SVN과 달리, 오프라인 개발이 가능하고, 효율적인 버전 관리를 제공하여 오픈소스를 더 쉽게 활용할 수 있게 하는 협업 툴

> Git 명령어
* git init : .git 디렉토리를 생성하는 명령어
* git clone : 다른 오픈소스 프로젝트 저장소를 복사해 가져오는 명령어
* git add 'file' : file을 저장소 준비 영역으로 보내주는 명령어
* git status : 현재 저장소 파일의 상태를 확인하는 명령어
* git commit -m 'add git' : 준비영역의 파일을 저장소에 반영하는 명령어
 
