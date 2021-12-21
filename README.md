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

### 크롤링 사이트

[https://finance.naver.com/news/news_search.naver]

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

- 다른 종목으로 돌리기
- json으로 만들어서
- 코드 중복제거하기
- [https://velog.io/@htchoi1006/중복기사-체크하기](https://velog.io/@htchoi1006/%EC%A4%91%EB%B3%B5%EA%B8%B0%EC%82%AC-%EC%B2%B4%ED%81%AC%ED%95%98%EA%B8%B0)
