<div align="center">

### Data Analyst | Data Engineering | SQL & Python

SQL과 Python을 활용해 데이터를 수집하고 정리하며,  
분석 가능한 형태로 구조화하는 과정에 관심이 있습니다.

데이터가 어떤 기준으로 쌓이고, 어떤 흐름으로 연결되며,  
어디에서 오류가 발생할 수 있는지를 함께 보는 편입니다.

이커머스 주문 데이터, 경기 이벤트 로그, 유전자 발현 데이터, 개인 운동 기록 등  
다양한 데이터를 다루며 전처리, 테이블 구조화, EDA, 모델링, 결과 해석까지 직접 수행해왔습니다.

</div>

<br>

<div align="center">

## 📚 Tech Stack

</div>

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-003B57?style=flat&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/ScikitLearn-F7931E?style=flat&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/CatBoost-FFCC00?style=flat&logoColor=black" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat&logoColor=white" />
</p>

<br>

---

## 📌 Main Projects

### 1. [Olist E-commerce Data Analysis](https://github.com/xxcxyxx/olist-ecommerce-analysis)

**SQL + Python 기반 이커머스 데이터 분석 프로젝트**

브라질 Olist 공개 데이터를 활용해 주문, 고객, 상품, 판매자, 결제, 리뷰 데이터를 SQLite DB로 구조화하고,  
SQL과 Python을 함께 사용해 배송 지연, 리뷰 점수, 고객 재구매, 지역별 주문 분포, 카테고리별 성과를 분석했습니다.

**Main Work**

- 원본 CSV 데이터를 SQLite DB로 적재
- 주문, 고객, 결제, 리뷰 등 주요 테이블 간 JOIN 분석
- SQL 기반 집계와 Python 기반 EDA 병행
- 배송 지연과 리뷰 점수 관계 분석
- 재구매 고객 비율 및 지역별 주문 집중도 분석

**Tech**

`SQL` `Python` `SQLite` `Pandas` `Matplotlib`

---

### 2. [2025 K League Pass Prediction](https://github.com/xxcxyxx/2025KLeaguePassPrediction)

**경기 이벤트 로그 기반 패스 도착 좌표 예측 프로젝트**

K리그 경기 이벤트 데이터를 `game_episode` 단위로 재구성하고,  
마지막 패스의 도착 좌표를 예측한 프로젝트입니다.

CatBoost, ExtraTreesRegressor, Ridge 모델을 비교하고  
OOF 기반 Optuna 가중 앙상블을 적용해 예측 성능을 개선했습니다.

**Main Work**

- 경기 이벤트 로그를 episode 단위로 재구성
- 마지막 패스 도착 좌표 `end_x`, `end_y` 예측
- CatBoost, ExtraTreesRegressor, Ridge 모델 비교
- OOF 기반 Optuna 가중 앙상블 적용
- 예측 오차 분포 및 공간 패턴 분석

**Tech**

`Python` `CatBoost` `Optuna` `scikit-learn`

---

### 3. [Lung Cancer Gene Prediction](https://github.com/xxcxyxx/Pre-training-with-Augmentation-Data-in-Deep-Learning-Model)

**유전자 발현 데이터 기반 폐암 아종 분류 딥러닝 프로젝트**

TCGA 폐암 유전자 발현 데이터를 활용해 폐암 아종을 분류하는  
MLP 기반 딥러닝 모델을 구현했습니다.

증강 데이터로 pre-training을 진행한 뒤,  
원본 데이터로 fine-tuning하는 2단계 학습 구조를 설계했습니다.

**Main Work**

- TCGA 폐암 환자 유전자 발현 데이터 활용
- 암 관련 유전자 323개 선별
- log2 변환 및 z-score 정규화
- PyTorch 기반 MLP 모델 구현
- Pre-training + Fine-tuning 구조 적용
- 최종 정확도 88.32%

**Tech**

`Python` `PyTorch` `NumPy`

---

### 4. [SQL Practice](https://github.com/xxcxyxx/solvesql)

**데이터 분석 직무 대비 SQL 문제 풀이 정리**

데이터 분석 직무에서 자주 활용되는 SELECT, JOIN, GROUP BY, 집계, 조건 처리 문제를 정리한 저장소입니다.  
문제 풀이뿐 아니라 쿼리 작성 의도와 풀이 흐름을 함께 정리하는 방식으로 관리하고 있습니다.

**Main Work**

- SolveSQL 문제 풀이 정리
- SELECT, JOIN, GROUP BY, 집계 쿼리 연습
- 문제별 풀이 코드와 설명 정리
- 데이터 분석 직무 대비 SQL 학습 기록 관리

**Tech**

`SQL`

---

## 💼 Experience

### National Institute of Forest Science

산사태 위험도 연구 관련 데이터를 정리하고 검토하며,  
현장조사 자료와 시스템 데이터를 연계해 연구용 데이터셋 품질을 관리했습니다.

시계열·공간 데이터의 기준을 맞추고,  
누락값과 항목 기준을 검토하며 분석 가능한 형태로 데이터를 정리한 경험이 있습니다.

### Math Academy Assistant Teacher

학생별 오답 유형, 숙제 미완료 패턴, 테스트 결과를 바탕으로  
학습 상태를 파악하고 보완 문제를 제공했습니다.

학생별 취약 단원과 반복 실수 패턴을 확인하며  
맞춤형 학습 관리를 진행했습니다.

---

## 📫 Contact

- GitHub: [github.com/xxcxyxx](https://github.com/xxcxyxx)
- Email: co505123060@gmail.com
