# 활용 프롬프트

## 1. 데이터 수집

```
kyobo_book_scroll.py파일을 생성하고 파이썬 코드로 구현할 내용은 다음과 같습니다.

[https://store.kyobobook.co.kr/bestseller/total/annual](https://store.kyobobook.co.kr/bestseller/total/annual?page=2)?page={page number} 교보문고 2024년 종합연간베스트 페이지에서 리뷰 수가 500개 이상인 도서의 상세 페이지 URL을 수집하여 kyobo_book_url.csv 파일로 저장하는 Python 스크립트를 작성해주세요. 다음 요구사항을 반영해주세요:

1. Selenium과 BeautifulSoup을 사용하여 동적 페이지를 크롤링
2. 각 도서의 상세 페이지를 방문하여 리뷰 수를 확인
3. 리뷰 수는 span.review_desc 요소에서 "(숫자개의 리뷰)" 형식으로 추출
4. 여러 방법으로 리뷰 수를 추출할 수 있도록 대비책 마련 (제목과 리뷰 수를 정확히 추출할 수 있는 다양한 방법 구현)
5. 여러 방법 중 하나에서 성공하면 다음 방법은 더이상 실행안하도록 코드 구현
6. 리뷰 수가 500개 이상인 도서만 선별하여  homework/data/ 폴더에 kyobo_book_url.csv파일에 저장하도록 구현
7. CSV 파일에는 도서 제목, 상세페이지 URL, 리뷰 수 정보가 포함되어야 함
8. 적절한 예외 처리와 로깅 기능 구현
9. page_number는 1~10까지 존재함
10. 파이썬 코드에는 적절히 주석을 추가해야 함
11. homework 폴더에 kyobo_book_scroll.py 라는 Python 스크립트를 작성해서 저장할것
12. 스크립트에 필요한 라이브러리는 selenium, pandas, requests, bs4, webdriver-manager입니다.
```
```
homework/data/경로에 kyobo_book_url.csv 파일에서 중복된 내용은 제거하고 도서코드 컬럼을 추가해서 homework/data/경로에 kyobo_book_list.csv 파일에 저장해주는 파이썬 스크립트를 작성해주세요
```
```
homework/data/경로에 kyobo_book_list.csv 파일에 도서코드를 이용하여 ch03/ref/scraper_kyobo.py 코드를 이용하여 리뷰정보를 추출하는 코드를 작성해주세요
```