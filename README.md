## [Dacon] AI프렌즈 시즌1 온도 추정 경진대회

기간 : 2020.03.01. ~ 2020.04.13.<br>
결과 : 
  - public : 1.47521 (대회 4등)
  - private : 3.51084 (대회 2등)
---
## 프로젝트 설명

### 요약 : 시계열 변수르 고려한 Feature Engineering과 LGBM & Ensemble을 적용항 모델 개발

### Feature Engineering

데이터의 모드 변수가 시계열 변수(기온, 현지기압, 풍속, 강수량, 해면기압, 일사량, 습도, 풍향)였음.
=> 해당 변수에 이동평균을 적용하여 Feature를 만듦.

### Modeling

![IMG_0011](https://user-images.githubusercontent.com/47520920/170411988-0f58dc70-febd-46a2-b6e9-30168a233041.JPG)

Feature Engineering으로 만든 Feature를 활용하여 5개의 Featureset을 만듦.

'Featureset 1 ~ 3(Power Mean Ensemble) + Featureset 4 + Featureset 5' 형태의 Ensemble을 통해 최종 모델 개발
