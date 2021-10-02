# `TEANAPS` Naver Cafe Post Scrapper

> `TEANAPS` Naver Cafe Post Scrapper는 네이버 카페 게시글 및 댓글 수집을 위한 웹스크래핑(크롤링) 도구입니다. 네이버 카페 내 검색결과를 수집 대상으로 하며 키워드 검색으로 원하는 기간, 게시판 대상으로 데이터 수집이 가능합니다. 본 자료는 수십만 개 이상의 네이버 카페 게시글을 수집하며 테스트 및 최적화를 진행하여 안정된 데이터 수집을 지원합니다. 직접 네이버 카페 데이터를 수집하고 [`TEANAPS`](https://github.com/fingeredman/teanaps#teanaps-text-analysis-apis-for-ecucation)를 활용해 텍스트 분석에 활용해보세요.

- 본 자료는 텍스트 마이닝을 활용한 연구 및 강의를 위한 목적으로 제작되었습니다.
- 본 자료를 강의 또는 연구 목적으로 활용하고자 하시는 경우 꼭 아래 메일주소로 연락주세요.
- 본 자료에 대한 <U>상업적 활용과 허가되지 않은 배포를 금지</U>합니다.
- 강의, 저작권, 출판, 특허, 공동저자에 관련해서는 문의 바랍니다.
- **Contact : ADMIN(admin@teanaps.com)**

---
## User Guide

### 1. 수집할 카페 게시글 검색

- 네이버에 로그인 후 수집대상 카페로 이동합니다.
- 카페 검색기능을 활용하여 내가 수집할 게시글을 검색합니다.
- 검색결과 페이지번호 링크를 복사하여 수집 URL을 확보합니다.

  > https://cafe.naver.com/dieselmania?iframe_url=/ArticleSearchList.nhn%3Fsearch.clubid=11262350%26search.media=0%26search.searchdate=all%26userDisplay=15%26search.option=0%26search.sortBy=date%26search.searchBy=0%26search.query=%C3%BB%B9%D9%C1%F6%26search.viewtype=title%26search.page=
  > - 여기서 페이지 번호는 제거하고 활용됩니다. (URL = "~search.page=")

### 2. 수집할 카페 검색결과 정보입력

- 아래 코드에서 수집할 카페 검색결과 정보를 입력합니다.

  > Python Code (in Jupyter Notebook) :
  > ```python
  > # 수집할 카페 검색결과 정보를 입력합니다.
  >                                    # 네이버 카페에서 게시글을 검색하고 검색결과 URL을 입력합니다.
  >                                    # URL은 네이버 카페에서 게시글 검색 후 검색결과 페이지 번호의 링크를 복사하여 찾을 수 있습니다.
  >                                    # 전체 URL에서 맨 뒤 페이지 번호는 제거하고 입력합니다. (URL = "~search.page=")
  > URL = "https://cafe.naver.com/dieselmania?iframe_url=/ArticleSearchList.nhn%3Fsearch.clubid=11262350%26search.media=0%26search.searchdate=all%26userDisplay=15%26search.option=0%26search.sortBy=date%26search.searchBy=0%26search.query=%C3%BB%B9%D9%C1%F6%26search.viewtype=title%26search.page="
  > PAGE_LIMIT = 3                     # 검색결과 중 수집할 최대 페이지 수를 입력합니다. (검색결과 페이지 수 보다 적게 입력)
  > POST_LIMIT = 5                     # 수집할 최대 게시글 수를 입력합니다.
  > SAVE_FILENAME = "cafe_post.txt"    # 수집결과를 저장할 파일명을 입력합니다.
  > ``` 

### 3. 수집시작

- 1~2번 과정 준비가 완료되면 전체 코드를 실행합니다. [[수집 데이터 정보(Excel)](https://github.com/fingeredman/teanaps-web-scrapper/raw/main/cafe_post_scrapper/sample_data/scrapping_data_desc.xlsx)]

---
## Release history
> 2021.10.02. `teanaps-cafe-post-scrapper v1.0.0` 업데이트   

---
## Update History
> 2021.10.02. 기본 구성 입력  

<br><br>
---
<center>ⓒ 2021. TEANAPS rights reserved.</center>
