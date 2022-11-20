# 경마 데이터 분석을 통한 경마 경기 결과 예측

## 진행 일정 (22.11.08 ~ 22.11.18)

### 1. 주제
경마 데이터 분석을 통한 경마 경기 결과 예측

### 2. 목적 및 시나리오
경마의 다양한 데이터를 사용하여 코로나로 축소됬던 경마 산업을 살리기 위하여 쉽게 접근 할수 있는 경마 결과 예측 모델을 만드는 것
<br><img width="60%" src="https://user-images.githubusercontent.com/95950967/202893604-8aa772df-d0cb-4304-ab7d-d3dd385fe6f9.jpg"/>

### Tech Stack
<div align=left> 
 <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
 <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> 
 <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">

## 분석 진행방향
### 1. 데이터 셋 구축 
- 출처 : 마사회 (http://kra.co.kr/)
- 기간 : 2022.11.11 ~ 2022.11.14
- 수집 내용
    1. 부마 / 모마 데이터
    2. 경주마 등급 데이터
    3. 경주마 경기 성적 데이터
    4. 현직 경주마 목록 데이터
    5. 조교사 데이터
    6. 기수 데이터    

### 2. 공모전 참여 인원 및 역할 
|                이름                      |               역할              |
| :-------------------------------:        | :----------------------------: |
|  [심재만](https://github.com/shimjaeman)  |     데이터 크롤링 및 모델링      |
|  [권효은](https://github.com/)            |     데이터 전처리 및 PPT 제작    |
|  [박재원](https://github.com/)            |     데이터 크롤링 및 모델링      |
|  [이승희](https://github.com/)            |         Project Manager        |
|  [정진명](https://github.com/)            |     데이터 전처리 및 모델링      |
|  [최규광](https://github.com/)            |     데이터 크롤링 및 시각화      |

### 3. 데이터 컬럼 설명 
경주마 경기 예측에 사용할 컬럼의 특징 및 선정이유
<br><img width="60%" src="https://user-images.githubusercontent.com/95950967/202894103-e444e1a6-6fd8-4b7b-ac62-55fb9c012355.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894037-d5b0f81d-25ee-419e-a969-e2ba9dd9349d.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894042-266484e2-5800-46b6-b8bc-932f7f66c8b4.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894041-4720bda0-b6f6-410d-995b-facf9a167501.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894040-08d005fd-b540-4680-9ea9-ddc86093ff67.jpg"/><br>

### 4. 데이터 전처리
Scoring / Null 처리 / Scaling / Encoding 
<br><img width="60%" src="https://user-images.githubusercontent.com/95950967/202894267-2b9135e5-32aa-4bd8-aa9a-5517c188077e.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894265-679f9c15-3986-4a03-adb9-58837fe05d03.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894264-945298e8-bca0-4d9b-829b-ffe0364faca1.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894262-cf60a5c9-c5dd-43a5-aee0-e84f42dd08ec.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894260-45d4bcf6-299d-4218-b786-cc9e1cc2acf9.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894257-11e3e629-39b6-4bac-a4e1-4e8aaac2b05d.jpg"/><br>

### 5. 모델 후보 및 성능지표
경마 경기 결과를 예측하는 모델을 만들기 때문에, 예측 결과가 얼마나 정확한지가 중요 -> Precision
<br><img width="60%" src="https://user-images.githubusercontent.com/95950967/202894599-f7d2a8d9-1f70-426a-8cfb-6dcab2295b27.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894601-123c7356-6f21-4dab-afab-6db877bfab26.jpg"/><br>

### 6. 모델링 
원래 여러 모델을 Voting해서 결정하기로 하였으나 다른 모델들의 과적합이 너무 심해서 RandomForest 모델만을 사용
<br><img width="60%" src="https://user-images.githubusercontent.com/95950967/202894867-38fdeab0-182f-4376-af43-f7c8c284ca8b.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894865-e2f3b349-a339-4985-893d-5c621d01a21f.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894862-2de0965c-169a-443a-94af-0912c709568c.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894861-eee4f433-5818-498e-93e2-bf5355e3b948.jpg"/>
<img width="60%" src="https://user-images.githubusercontent.com/95950967/202894857-8140ae8f-7644-4641-80a1-ad51c014f24b.jpg"/><br>

## 최종 결과
<br><img width="100%" src="https://user-images.githubusercontent.com/95950967/202895014-4f3bea41-d02a-4bd9-9252-39ad216ed27e.jpg"/><br>


## 참고논문 및 사이트
*
