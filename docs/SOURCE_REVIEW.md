# 2026-10-21 강의 자료 검토
자료 위치: 사용자가 공유한 부경대학교 AI Campus Drive 폴더. 공개 학습 Git에서는 원본 교재, 수업 코드, Drive 직접 링크, 학생 자료를 재배포하지 않는다.

## 확인 파일
- 1day_Python_리뷰 / 1day_리뷰.txt
- 2day_Data_Preprocess / 01_data_preprocessing.ipynb
- 3day_Feature_Enginnering / 3day_Feature_Enginnering.ipynb
- 4day_Feature_Enginnering / 4day_Feature_Enginnering.ipynb
- 5day_Regression_Model_Base / 5day_regression_model_base.ipynb
- 6day_Linear_Regression_Model / 01_linear_regression_model.ipynb 등
- 7day_Polynomial_Features / 02_linear_regression_model.ipynb 및 03_regression_All_Model.ipynb
- UV_개발환경_메뉴얼.txt: Python 3.10과 uv 환경 구성 안내

## 반드시 보완할 내용
4일차 노트북은 전체 원본 데이터에 SMOTE.fit_resample을 먼저 적용하고, 그 합성 데이터를 train_test_split으로 분할한다. 이 순서는 데이터 누수를 일으킬 수 있고 평가 점수의 과대 추정 위험이 있다. 수정 실습에서는 먼저 원본을 train/validation/test로 분리한 뒤 훈련 데이터에만 SMOTE와 학습형 변환을 적용한다.
공식 참고: https://imbalanced-learn.org/stable/common_pitfalls.html

## 아직 검증하지 않은 항목
실제 수업의 8일차 이후 편성, 강의 코드의 성공 실행, 원본 데이터 라이선스, 개인 학습의 통과 여부, 로컬 실행 환경 및 Worktree.
