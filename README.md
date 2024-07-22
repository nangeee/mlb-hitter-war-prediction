# ⚾ mlb-hitter-war-prediction


## 💡 Project Introduction
FA Scouter는 머신러닝을 활용하여 야구 선수의 미래 성과를 예측하고 적절한 연봉을 계산하는 프로젝트입니다. 
주요 성과 지표로 Wins Above Replacement (WAR)를 사용하여 FA(자유계약선수) 선수의 연봉을 결정하는 데 도움을 주는 예측 모델을 개발하는 것을 목표로 합니다. 
다양한 모델을 비교하고 최적의 모델을 선택하여 선수의 미래 성과를 예측하고, 이를 기반으로 적절한 연봉을 제안합니다.


## 🪄 Project Timeline
2023.10 ~ 2023.12


## 🗝️ Technology Stack
**Development Environment**: Google Colab, Jupyter Notebook

**Programming Language**: Python

**Libraries**: scikit-learn, XGBoost, pandas, numpy, seaborn, matplotlib

**Data Source**: pybaseball library (Statcast, Baseball Reference, Fangraphs)


## 🎯 Key Activities
1. **Data Collection**
   - 'pybaseball' 라이브러리를 사용하여 1871년부터 2023년까지의 MLB 타자 통계를 수집

2. **Data Preprocessing**
   - 시즌 필터, 선수 필터, 커리어 분할, 압축 과정을 통해 데이터를 전처리
   - 시즌 및 선수 필터링, 커리어 분할, 데이터 압축을 통해 초기 데이터의 크기를 줄이고, 모델 훈련에 적합한 형태로 변환

3. **Exploratory Data Analysis (EDA)**
   - 데이터의 분포 및 특성 간의 관계를 이해하기 위해 시각화 도구를 사용하여 분석

4. **Feature Selection and Modeling**
   - SelectKBest, RFECV, PCA 등의 기법을 사용하여 특징 선택 및 차원 축소
   - Random Forest, XGBoost, Lasso 알고리즘을 사용하여 모델을 구축
  
5. **Model Evaluation and Insights**
   - 모델의 성능을 R-squared 점수 및 MAE로 평가
   - 선수의 연령, 최근 시즌 데이터, 과거 WAR 등의 특징이 미래 WAR 예측에 중요한 영향을 미친다는 인사이트를 도출
