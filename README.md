# DART PROJECT

## 📈 주가 변화에 따른 뉴스 제공 툴 구현

<aside>
💡 뉴스클러스터링으로 각 종목별 주가변화에 따른 대표 뉴스를 제공할 수 있는 기능을 구현하는 프로젝트. 한마디로 설명하자면 ‘이날 00은 왜 올랐을까?/ 내렸을까’ 를 시각화하는 것입니다.

</aside>

### Member

민시온, 구현아, 오수진, 장민지, 장창영

### Summary

- 클러스터링
- 시총 50위 종목에 대해 기능을 구현
- 이후 전체 종목 -> 웹구현까지도 계획!!

[👼 프로젝트 진행상황](https://www.notion.so/6b491e3de7ce4befad137c23bcc0f87a)

# 📚 공부한 내용들 정리/ 공유

bigkinds의 경우 get이 아닌 post 방식으로 크롤링해야할 듯

post 방식의 크롤링 : [https://surgach.tistory.com/6](https://surgach.tistory.com/6)   (참고)

[빅카인즈.ipynb](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/%EB%B9%85%EC%B9%B4%EC%9D%B8%EC%A6%88.ipynb)

[https://joon0zo.tistory.com/20#](https://joon0zo.tistory.com/20#)

[https://code-study.tistory.com/59?category=964015](https://code-study.tistory.com/59?category=964015)

[https://stickode.tistory.com/188](https://stickode.tistory.com/188) (코드 쉬움, 대신 페이지 넘기는거 x)

[https://m.blog.naver.com/htk1019/221008762101](https://m.blog.naver.com/htk1019/221008762101)

셀레니움 로그인

 .send_keys

### 크롤링 사이트

[https://finance.naver.com/news/news_search.naver?rcdate=0&q=�Ｚ����&x=30&y=6&sm=title.basic&pd=1&stDateStart=1997-01-01&stDateEnd=2021-12-16](https://finance.naver.com/news/news_search.naver?rcdate=0&q=%BB%EF%BC%BA%C0%FC%C0%DA&x=30&y=6&sm=title.basic&pd=1&stDateStart=1997-01-01&stDateEnd=2021-12-16)

### 

### DB만들면

뉴스 수집 넘버

종목 코드 

종목 이름

언론사 이름
뉴스 고유 코드(id)
기사제목
기사 요약내용
기사내용
기사에 사용된 이미지 경로
기사 URL
기사 입력일

수집 일시 

### 크롤링 형식

data = {

         'ticker_code' : 005930,     → 종목 티커

         'ticker_name' : 삼성전자,     → 종목 이름

               'media_code' : 1,                  → 언론사 식별번호
                'media_name' : '서울경제',  → 언론사 이름
                'news_code' : news_code, → 뉴스 고유 코드(id)
                'news_title' : title, → 기사제목
                'news_summary' : summary, → 기사 요약내용
                'news_thumb_url' : thumbnail_url, → 기사 이미지 경로(이미지는 맨 앞에 것만)
                'url' : news_url, → 기사 URL
                'news_reg_date' : regist_date → 기사입력일
            }

### 크롤링 날짜

2011/12/1 ~ 2021/12/1 → 그냥 우리가 편해서 ㅋㅋ

![Untitled](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/Untitled.png)

![Untitled](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/Untitled%201.png)

1~16: 민시온

[Crawling.ipynb](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/Crawling.ipynb)

- 다른 종목으로 돌리기
- json으로 만들어서
- 코드 중복제거하기
- [https://velog.io/@htchoi1006/중복기사-체크하기](https://velog.io/@htchoi1006/%EC%A4%91%EB%B3%B5%EA%B8%B0%EC%82%AC-%EC%B2%B4%ED%81%AC%ED%95%98%EA%B8%B0)

17~33: 오수진

[시총 17위~33위.ipynb](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/%EC%8B%9C%EC%B4%9D_17%EC%9C%8433%EC%9C%84.ipynb)

34~50: 장민지

## **ppt 얼개**

[다트 2021.2 프로젝트 발표.pptx](DART%20PROJECT%204b9d61e4c6ce444caec3acc44b15a8a4/%EB%8B%A4%ED%8A%B8_2021.2_%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8_%EB%B0%9C%ED%91%9C.pptx)
