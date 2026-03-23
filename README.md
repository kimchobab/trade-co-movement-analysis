# 국민대 AI 빅데이터 분석 경진대회
<img width="949" height="219" alt="스크린샷 2026-02-09 125018" src="https://github.com/user-attachments/assets/94acc5cb-021a-460a-8374-871d8f3e0fcd" />

[DACON](https://www.dacon.io/competitions/official/236619/overview/description)

-------------------------------------------------------------------------------------

## 1. 개요 및 목적
[프로젝트 설명] 원시 무역 수입 데이터(2022년 1월 ~ 2025년 7월)를 기반으로, 
품목 간 공행성(comovement)이 존재하는 선후행 쌍을 예측하고, 공행성이 있다고 판단된 경우에는 
후행 품목의 다음 달(2025년 8월) 총 무역량(value)을 예측하는 AI 모델을 개발합니다.

- 참가자는 주어진 원시 무역 데이터를 분석하여 품목 간 선후행 관계가 존재하는 공행성 쌍(A → B)을 찾고,
- 이후에는 선행 품목(A)의 흐름을 활용해 후행 품목(B)의 다음달의 총 무역량(value)을 예측해야 합니다.

## 2. 기술 스택 (Tech Stack)
| 구분 | 기술 |
|------|------|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Analysis | Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Environment | Google Colab |

## 2. Pipeline
1. import / 데이터 로딩
2. Preprocessing (전처리)
3. 변수 분포간 시각화
4. 변수간 관계 시각화
5. Analysis
   -a. 데이터 전처리
   -b. 변수 분석
   -c. 상관 관게 및 Feature Engineering
6. 공행성 후보 선정 및 공행성 쌍 데이터 탐색
7. 다음 후행 무역량 예측

## 3. 🚀 Key Results (핵심 성과)

## 4. 분석 프로세스 (Workflow)
1. **Data Cleaning**: 품목별 시계열 데이터 결측치 보간 및 정규화.
2. **Feature Engineering**: 선행 지표 도출 및 시계열 래그(Lag) 변수 생성.
3. **Statistical Testing**: 품목 쌍별 Granger Causality 검정 수행.
4. **Model Training**: 앙상블 모델을 활용한 차월 무역량 회귀 분석.
5. **Evaluation**: 검증 데이터셋을 활용한 오차 분석 및 하이퍼파라미터 최적화.

## 5. 기대 효과 및 활용 방안
* **공급망 관리**: 수입량 급감/급증에 대한 선행 지표를 확보하여 리스크 사전 대응 가능.
* **재고 최적화**: 후행 품목의 수요 예측 정확도를 높여 물류 비용 절감에 기여.

