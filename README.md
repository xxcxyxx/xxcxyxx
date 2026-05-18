<div align="center">

### Data Analyst | SQL & Python

SQL과 Python을 활용해 데이터를 정리하고,  
문제의 원인을 분석해 인사이트로 연결하는 데이터 분석가를 목표로 하고 있습니다.

데이터를 바로 결론으로 연결하기보다,  
먼저 구조와 기준을 확인하고 분석 가능한 형태로 정리하는 과정을 중요하게 생각합니다.

이커머스 주문 데이터, 경기 이벤트 로그, 유전자 발현 데이터 등  
다양한 데이터를 다루며 전처리, EDA, 지표 분석, 모델링, 결과 해석까지 직접 수행해왔습니다.

</div>

<br>

<div align="center">

## 📚 Tech Stack

</div>

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-003B57?style=flat&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/CatBoost-FFCC00?style=flat&logoColor=black" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" />
</p>

<br>

---

## 📌 Main Projects

### 1. [Olist E-commerce Data Analysis](https://github.com/xxcxyxx/olist-ecommerce-analysis)

**SQL + Python 기반 이커머스 고객·배송·매출 데이터 분석 프로젝트**

브라질 Olist 공개 데이터를 활용해 주문, 고객, 상품, 결제, 리뷰, 배송 데이터를 분석했습니다.  
총 99,440건의 주문 데이터를 SQLite DB에 적재하고, SQL과 Python을 활용해 월별 주문·매출 흐름, 고객 재구매율, 배송 지연과 리뷰 점수의 관계, 카테고리별 성과 차이를 분석했습니다.

**Main Work**

- 원본 CSV 데이터를 SQLite DB로 적재하고 주요 테이블 구조 확인
- SQL 기반 월별 주문 수, 매출, 고객별 주문 횟수, 배송 지연 여부 집계
- Python pandas 기반 전처리 및 matplotlib 시각화
- 재구매율, 배송 지연율, 리뷰 점수 차이, 카테고리별 주문·매출 비교 분석
- 분석 결과를 README와 SQL 파일로 문서화

**Key Results**

- 전체 주문 **99,440건** 분석
- 총 매출 **16,008,872.12** 확인
- 고유 고객 **96,096명** 중 재구매 고객 **2,997명**, 재구매율 **3.12%**
- 배송 지연 주문 **6,535건**, 배송 지연율 **6.77%**
- 정상 배송 평균 리뷰 **4.29점**, 지연 배송 평균 리뷰 **2.27점**으로 **2.02점 차이** 확인
- 주문 수 1위 카테고리 `bed_bath_table`, 매출 1위 카테고리 `health_beauty`로 주문량과 매출 기여도의 차이 확인

**Tech**

`SQL` `Python` `SQLite` `pandas` `Matplotlib` `Jupyter Notebook`

---

### 2. [2025 K League Pass Prediction](https://github.com/xxcxyxx/2025-K-League-Pass-Prediction)

**K리그 이벤트 로그 데이터 분석 및 패스 좌표 예측 프로젝트**

K리그 경기 이벤트 로그를 `game_episode` 단위로 재구성하고, 마지막 패스 도착 좌표를 예측한 프로젝트입니다.  
원본 이벤트 로그 356,721건을 15,428개 episode 학습 샘플로 변환하고, CatBoost·ExtraTrees·Ridge 모델 비교와 OOF 기반 앙상블을 적용했습니다. 이후 예측 오차 분포와 공간별 오차 패턴을 분석했습니다.

**Main Work**

- 경기 이벤트 로그를 `game_episode` 기준 학습 데이터로 재구성
- episode별 이벤트 수, 액션 유형, 성공 여부, 좌표 통계량, 이동 거리 기반 feature 생성
- CatBoost, ExtraTrees, Ridge 모델 비교
- OOF 기반 Optuna 가중 앙상블 적용
- Mean/Median/P90 Error 기준 예측 오차 분포 분석
- Error Heatmap, Error Vector 시각화를 통한 공간별 오차 패턴 해석

**Key Results**

- 원본 이벤트 로그 **356,721건** → episode 단위 학습 샘플 **15,428개**로 재구성
- 최종 OOF ensemble score **18.9466** 기록
- Median Error **16.3242m**, P90 Error **35.5961m** 기준 오차 분포 분석
- CatBoost 단일 모델 대비 OOF 앙상블로 validation 기준 성능 소폭 개선
- 특정 공간 구역에서 오차가 커지는 패턴을 확인해 모델의 취약 구간 해석

**Tech**

`Python` `pandas` `CatBoost` `ExtraTrees` `Ridge` `Optuna` `scikit-learn` `Matplotlib`

---

### 3. [Lung Cancer Gene Expression Classification](https://github.com/xxcxyxx/Lung-Cancer-Gene-Expression-Classification)

**유전자 발현 데이터 기반 폐암 아종 분류 및 증강 학습 실험 프로젝트**

TCGA 폐암 유전자 발현 데이터를 활용해 폐암 아종을 분류하고, 데이터 증강 기반 2단계 학습 구조의 효과를 검증한 프로젝트입니다.  
환자 1,018명, 원본 유전자 19,977개로 구성된 고차원 데이터를 다뤘으며, 암 관련 유전자 323개를 선별한 뒤 log2 변환과 z-score 정규화를 수행했습니다.

**Main Work**

- TCGA 폐암 유전자 발현 데이터 전처리
- 원본 유전자 19,977개 중 암 관련 유전자 323개 선별
- log2 변환 및 z-score 정규화를 통한 발현값 분포·스케일 보정
- PyTorch 기반 MLP 모델 구현
- 증강 데이터 pre-training → 원본 데이터 fine-tuning 2단계 학습 구조 설계
- Stratified 10-fold Cross Validation 기반 성능 검증
- 실험 결과를 논문 형태로 문서화

**Key Results**

- TCGA 폐암 환자 데이터 **1,018명** 분석
- 원본 유전자 **19,977개** 중 암 관련 유전자 **323개** 선별
- 최종 분류 정확도 **88.32%** 기록
- Baseline MLP 대비 약 **1% 성능 향상** 확인
- 소량·고차원 의료 데이터에서 전처리와 학습 전략 설계의 중요성 확인

**Tech**

`Python` `PyTorch` `pandas` `NumPy` `scikit-learn` `MLP` `Jupyter Notebook`

---

### 4. [SQL Practice](https://github.com/xxcxyxx/solvesql)

**데이터 분석 직무 대비 SQL 문제 풀이 정리**

데이터 분석 직무에서 자주 활용되는 SELECT, JOIN, GROUP BY, 집계, 조건 처리 문제를 정리한 저장소입니다.  
문제 풀이뿐 아니라 쿼리 작성 의도와 풀이 흐름을 함께 정리하며 SQL 분석 역량을 꾸준히 보완하고 있습니다.

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

학생별 취약 단원과 반복 실수 패턴을 확인하며,  
데이터 기반으로 문제 원인을 파악하고 개인별 개선 방향을 제안했습니다.

---

## 🔎 What I Focus On

- SQL과 Python을 활용한 데이터 정리 및 분석
- 여러 테이블 간 관계 이해와 JOIN 기반 분석
- EDA를 통한 문제 원인 파악
- 수치와 시각화를 활용한 분석 결과 설명
- 데이터 기반 인사이트 도출 및 문서화
- 분석 결과를 현업이 이해할 수 있는 형태로 정리

---

## 📫 Contact

- GitHub: [github.com/xxcxyxx](https://github.com/xxcxyxx)
- Email: co505123060@gmail.com
