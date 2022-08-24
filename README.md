<p align="center">
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcRZyWw%2FbtrJ2nbV0Ly%2FV0thL6tNjJKnkPrHsiYlJK%2Fimg.png">
</p>

# 📖[웹소설] 일타강사 AI의 기막힌 추천 (웹타추)

## INTRO
* 네이버 시리즈에서 판매중인 웹소설 작품의 작품정보를 크롤링한 데이터를 기반으로
* 자연어 처리를 이용해 웹소설의 스토리들을 벡터 임베딩 하여
* 사용자가 좋아요를 누른 소설의 줄거리와 유사도가 높은 작품을 추천해주는 서비스를 제공하는 웹사이트

### Team
|이름|역할|깃허브|
|:---:|---|---|
|김동근|메인 페이지, 장르별 페이지|[![github_icon](https://img.shields.io/badge/Github-000000?style=flat-square&logo=github&logoColor=white)](https://github.com/yinmsk)|
|노을|로그인 페이지, 마이 페이지|[![github_icon](https://img.shields.io/badge/Github-000000?style=flat-square&logo=github&logoColor=white)](https://github.com/minkkky)|
|이정아|작품 상세 페이지|[![github_icon](https://img.shields.io/badge/Github-000000?style=flat-square&logo=github&logoColor=white)](https://github.com/zeonga1102)|
|이현경|작품 상세 페이지|[![github_icon](https://img.shields.io/badge/Github-000000?style=flat-square&logo=github&logoColor=white)](https://github.com/LULULALA2)|

* 추천 모델 제작은 다 같이 한다.

### S.A 
* [블로그로 이동(☞ﾟヮﾟ)☞](https://cold-charcoal.tistory.com/85)
---

## PROJECT

### Feature
* 회원가입 및 로그인 - 장고 내장 모델 사용
* 작품 제목을 기준으로 검색하는 기능
* 선호작을 누른 작품들의 스토리와 유사도가 높은 작품들을 추천, 선호작을 아직 누르지 않았다면 별점이 높은 작품들을 추천
* Today best top 20 - 네이버 시리즈의 일간 Top100에서 20위까지 크롤링해서 보여주기
* 장르별 페이지에서 작품들을 페이지네이터를 이용해 보여주기
* 작품 상세 페이지에서 댓글들의 키워드를 분석해서 가장 많은 키워드 5개 표시
* 선호작 기능
* 리뷰 작성, 조회, 수정, 삭제
* 마이 페이지에서 선호작 누른 작품들의 스토리 키워드 빈도수 상위 10개 표시
* 사용자의 선호작 5개와 작성한 리뷰들을 일부 보여주고 전체보기로 모든 항목들 표시

### Architecture
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=fff) ![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=fff) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=python&logoColor=fff) ![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=fff) ![MeCab](https://img.shields.io/badge/MeCab-000?style=for-the-badge) ![Doc2Vec](https://img.shields.io/badge/Doc2Vec-000?style=for-the-badge)

### DB(ERD)
![image](https://user-images.githubusercontent.com/104331869/185334447-e9eaabb2-c3e0-4d1a-95de-5bb09921b73a.png)

### Preview
* [시연 영상 확인하기(☞ﾟヮﾟ)☞](https://moist-ink.tistory.com/entry/webtachu)

|![image](https://user-images.githubusercontent.com/104331869/185335939-524bba9a-0f3c-46a1-bd07-628a852fbab2.png)|![image](https://user-images.githubusercontent.com/104331869/185335986-2b364717-cbd4-4d6b-9d8d-402d934dfaab.png)|![image](https://user-images.githubusercontent.com/104331869/185336258-a03c1dc7-d0c8-450b-8db2-bf3b6d94ec27.png)|![image](https://user-images.githubusercontent.com/104331869/185336306-f071016c-1077-445c-98e0-03f19b8cf29e.png)|
|:---:|:---:|:---:|:---:|
|로그인|회원가입|메인 페이지|장르별 작품 리스트|
|![image](https://user-images.githubusercontent.com/104331869/185338031-62118c95-2fd7-4860-b2da-75ae1f22fcaf.png)|![image](https://user-images.githubusercontent.com/104331869/185337856-1f08eb63-35d1-4712-8d2a-0a13cbaa16a0.png)|![image](https://user-images.githubusercontent.com/104331869/185338071-2d4bd6e3-3b71-4bf8-9525-41ee2b988a0f.png)|![image](https://user-images.githubusercontent.com/104331869/185338306-4d1e7365-9d8c-47bc-ba02-c855c837b2d3.png)|
|검색 결과|작품 상세 페이지|마이 페이지|나의 리뷰 모아보기|

### Credit
* [네이버 시리즈](https://series.naver.com/novel)
