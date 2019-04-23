# R Basic

### 설치
* R
  * https://cran.r-project.org/ 방문
  * 해당 OS 최신 버전 다운로드
  * R은 Python을 설치하기 위해 Anaconda를 설치한다고 이해하면 됨

* R Studio
  * https://www.rstudio.com/ 방문
  * 해당 OS 최신 버전 다운로드 (RStudio Desktop Open Source License, Free)

### 실행
* R Studio 실행
  * Win : 시작메뉴 > R Studio
  * Mac : Application > R Studio

### RStudio 기본 화면 사용법
* Console
  * 프롬프트 방식으로 명령을 순차적으로 입력하면서 사용(Jupyter Notebook/Lab과 유사)
  * 패키지(라이브러리) 설치 가능
* File Edit
  * R 스크립트 파일을 편집하여 실행 가능
  * 일반적인 에디터 기능
* Histody
  * 그동안 실행한 명령 히스토리를 확인할 수 있음
* Plots
  * 챠트, 이미지 등 생성 시 표시되는 영역
  * 이미지 파일이나 PDF, 클립보드로 복사 가능
* Packages
  * 전체 패키지 목폭, 설치된 패키지 목록 확인 가능
  * 패키지를 설치하거나 삭제할 수 있음

### R Package
* 설치
  ```
  install.packages(패키지명)
  ```
* 업데이트
  ```
  update.packages(패키지명)
  ```
* 로드
  ```
  library(패키지명)
  ```

### 파일 입/출력 및 확인
* CSV 파일 입력받아 데이터프레임에 저장
  ```
  train <- read.csv("./DataScience/03_study/01_pulip_study_data_science/data_titanic/train.csv", header = TRUE)
  ```
* 데이터프레임 확인
  ```
  head(train)
  tail(train)
  ```
* 데이터프레임 뷰
  ```
  View(train) # 대소문자 구분
  ```
### 그래프
* 산점도
  ```
  plot(train$Age, train$Fare)
  ```
* 상자그림
  ```
  boxplot(train$Age)
  ```)
* 히스토그램
  ```
  hist(train$Age)
  ```
### 벡터 평균, 분산, 표준편차
* 분산 : 각 편차 제곱의 합의 평균
* 편차 : 평균과의 차이
* 표준편차 : 루트분산(분산이 제곱값이라 실질적인 치우침에 비해 값이 커서 루트를 씌움)
```
a = 1:10
a
[1]  1  2  3  4  5  6  7  8  9 10
mean(a) # 평균
[1] 5.5
var(a) # 분산(variance)
[1] 9.166667
sd(a) # 표준편차
[1] 3.02765
```
* *** 합, 중앙값, 자연로그값
```
sum(a)
[1] 55
median(a)
[1] 5.5
log(a)
[1] 0.0000000 0.6931472 1.0986123 1.3862944 1.6094379 1.7917595 1.9459101 2.0794415
[9] 2.1972246 2.3025851
```

### R을 활용한 Titanic data 분석 기초 과정 - Kaggle
* https://www.kaggle.com/redhorse93/r-titanic-data