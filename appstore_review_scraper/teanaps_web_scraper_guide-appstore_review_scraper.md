# `TEANAPS` AppStore Review Scrapper

> `TEANAPS` AppStore Review Scrapper는 앱스토어에 등록된 앱 리뷰 수집을 위한 웹스크래핑(크롤링) 도구입니다. 본 자료는 다양한 프로젝트 및 논문작성에 활용하며 테스트 및 최적화를 진행하여 안정된 데이터 수집을 지원합니다. 직접 앱스토어 리뷰 데이터를 수집하고 [`TEANAPS`](https://github.com/fingeredman/teanaps#teanaps-text-analysis-apis-for-ecucation)를 활용해 텍스트 분석에 활용해보세요.

- 본 자료는 텍스트 마이닝을 활용한 연구 및 강의를 위한 목적으로 제작되었습니다.
- 본 자료를 강의 또는 연구 목적으로 활용하고자 하시는 경우 꼭 아래 메일주소로 연락주세요.
- 본 자료에 대한 <U>상업적 활용과 허가되지 않은 배포를 금지</U>합니다.
- 강의, 저작권, 출판, 특허, 공동저자에 관련해서는 문의 바랍니다.
- **Contact : ADMIN(admin@teanaps.com)**

---
## User Guide

### 1. Install Selenium

- [Selenium](https://pypi.org/project/selenium/) - *pip install selenium*

  > Python Code (in Jupyter Notebook) :
  > ```python
  > !pip install selenium
  > ```

### 2. Chrome Driver Setting

- 자신의 PC에 설치된 Chrome 브라우저에 맞는 Chrome Driver 버전을 다운로드합니다. [[Chrome Driver 다운로드](http://chromedriver.chromium.org/downloads/)]
- 다운로드한 Chrome Driver 파일 경로를 아래 코드의 `DRIVER_PATH`에 입력합니다.

  > Python Code (in Jupyter Notebook) :
  > ```python
  > # Windows 운영체제
  > #DRIVER_PATH = "chromedriver.exe"
  > 
  > # MAC, Linux 운영체제
  > # - 경고메시지 출력 시 보안 및 개인정보보호 메뉴에서 "확인없이 허용" 클릭 필요함
  > DRIVER_PATH = "./chromedriver"
  > ```
 
### 3. 수집할 리뷰 정보입력

- 아래 코드에서 수집할 리뷰 정보를 입력합니다.

  > Python Code (in Jupyter Notebook) :
  > ```python
  > # 수집할 리뷰 페이지 URL 정보를 입력합니다.
  > URL = "https://apps.apple.com/kr/app/%EC%8B%A0%ED%95%9C%ED%8E%98%EC%9D%B4%ED%8C%90/id572462317#see-all/reviews"
  > 
  > # 스크롤을 내릴 횟수를 입력합니다.
  > # 스크롤을 여러번 내릴수록 더 많은 리뷰가 수집됩니다.
  > SCROLL_COUNT = 5
  > 
  > # 리뷰를 저장할 파일명
  > REVIEW_FILENAME = "appstore_review.txt"
  > ``` 

### 4. 수집시작

- 1~3번 과정 준비가 완료되면 전체 코드를 실행합니다. [[수집 데이터 정보(Excel)](https://github.com/fingeredman/teanaps-web-scrapper/raw/main/appstore_review_scrapper/sample_data/scrapping_data_desc.xlsx)]

  > ![scrapping_sample](./sample_data/scrapping_sample.gif)

---
## Release history
> 2021.07.10. `teanaps-appstore-review-scrapper v1.0.0` 업데이트  

---
## Update History
> 2021.07.10. `User Guide` 업데이트  
> 2021.05.30. 기본 구성 입력  

<br><br>
---
<center>ⓒ 2021. TEANAPS rights reserved.</center>
