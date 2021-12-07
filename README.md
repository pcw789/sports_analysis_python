# 스포츠 데이터 분석


## Description

스포츠 경기(MLB, EPL)에서 발생한 데이터를 활용해 팀의 승률 예측, 선수 가치 평가 등의 분석을 수행하였다.

## 득점 및 실점과 팀의 승률과의 관계성(피타고리안 승률) 분석

### Description

* (득점)^2  / [ (득점)^2 + (실점)^2 ] 의 수식값이 승률과 비례한다는 이론.
* 어떤 스포츠에도 성립.

### EPL과 MLB 경기 기록 데이터 분석

* [EPL 17-18](https://github.com/pcw789/sports_analysis_python/blob/main/EPL_Pythagorean_Predictor.ipynb)
* [MLB 16](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_Pythagorean_predict.ipynb)

### 분석

* 각 팀별 득점과 실점 기록으로 피타고리안 값을 계산
* 피타고리안 값과 팀의 승률을 Scatter Plot으로 표현
* Linear Regression으로 피타고리안 값이 승률에 미치는 영향 분석

## Run Value 분석

### Description

* 야구의 득점 기여도에 대한 분석.
* 선수가 팀의 득점에 얼마나 기여했는가를 측정(Run Value).
* 팀의 종합 Run Value가 승률과 얼마나 연관이 있는가 분석(Linear Regression).

### MLB 경기 기록 데이터 분석

* [MLB 17](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_Run_Expectancy.ipynb)

### 분석

* 야구에 존재하는 모든 타석 상황에 대한 기대 득점을 계산한다.(Run Expectancy)
* 각 타자들이 들어선 타석 상황(기대 득점)에서 얼마나 활약했는지 측정한다.(Run Value)
   * ex) 0아웃 0주자 상황의 Run Expectancy = 0.498
   * ex) 0아웃 1주자 상황의 Run Expectancy = 0.913
   * ex) 타자가 0아웃0주자에서 출루해 0아웃1주자 상황을 만듦 => Run Value = 0.913 - 0.498 = 0.415


## 파워형 투수 vs 기교파 투수

### Description

* 파워형 투수(Power Pitcher)와 기교파 투수(Finesse Pitcher) 유형별 성적 특징 분석.

### 경기 기록 데이터 분석

* [Power Vs Finesse](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_Pitcher_Data(Power_vs_Finesse).ipynb)

### 분석

* PFR 수치를 계산하여 투수를 파워형과 기교파로 분류 [ PFR = ( K + BB ) / IP ]
* PFR 수치 상위 25%(Power)와 하위 25%(Finesse)를 기록한 투수들의 성적 비교




