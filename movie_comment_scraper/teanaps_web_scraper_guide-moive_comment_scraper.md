# `TEANAPS` Movie Review Scraper

> `TEANAPS` Movie Review Scraper는 네이버 뉴스기사 및 댓글 수집을 위한 웹스크래핑(크롤링) 도구입니다. 네이버 뉴스기사 검색결과를 수집 대상으로 하며 키워드 검색으로 원하는 기간, 개수 만큼 뉴스기사 데이터수집이 가능합니다. 본 자료는 10년치 이상의 뉴스기사를 수집하며 테스트 및 최적화를 진행하여 안정된 데이터 수집을 지원합니다. 직접 뉴스기사 데이터를 수집하고 [`TEANAPS`](https://github.com/fingeredman/teanaps#teanaps-text-analysis-apis-for-ecucation)를 활용해 텍스트 분석에 활용해보세요.

- 본 자료는 텍스트 마이닝을 활용한 연구 및 강의를 위한 목적으로 제작되었습니다.
- 본 자료를 강의 또는 연구 목적으로 활용하고자 하시는 경우 꼭 아래 메일주소로 연락주세요.
- 본 자료에 대한 <U>상업적 활용과 허가되지 않은 배포를 금지</U>합니다.
- 강의, 저작권, 출판, 특허, 공동저자에 관련해서는 문의 바랍니다.
- **Contact : ADMIN(admin@teanaps.com)**

---
## User Guide

### 1. 수집할 영화코드 확인

- 네이버 영화 페이지에서 수집대상 영화 페이지에 접속합니다.
- 해당 영화 페이지 URL에서 영화코드를 확인합니다.

  > https://movie.naver.com/movie/bi/mi/basic.nhn?code=189150
  > - 여기서 영화코드는 "189150" 입니다.

### 2. 수집할 영화리뷰 정보입력

- 아래 코드에서 수집할 영화리뷰 정보를 입력합니다.

  > Python Code (in Jupyter Notebook) :
  > ```python
  > # 수집할 영화리뷰 정보를 입력합니다.
  > PAGE_LIMIT = 10                         # 수집할 영화리뷰 페이지 개수
  > SAVE_FILE_PATH = "movie_comment.txt"    # 영화리뷰 저장 파일명
  > MOVIE_CODE = 194205                     # 영화 코드
  > ``` 

### 3. 수집시작

- 1~2번 과정 준비가 완료되면 전체 코드를 실행합니다. [[수집 데이터 정보(Excel)](https://github.com/fingeredman/teanaps-web-scraper/raw/main/movie_comment_scraper/sample_data/scraping_data_desc.xlsx)]

---
## Release history
> 2021.07.03. `teanaps-movie-comment-scraper v1.0.0` 업데이트   

---
## Update History
> 2021.07.03. 기본 구성 입력  

<br><br>
---
<center>ⓒ 2021. TEANAPS rights reserved.</center>
