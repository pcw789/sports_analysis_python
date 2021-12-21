# 스포츠 데이터 분석


## Description

스포츠 경기에서 발생한 데이터를 활용해 데이터 분석을 수행하였다.

<br/>
<br/>

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

<br/> 
<br/>

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
   * ex) 타자가 0아웃0주자에서 출루해서 0아웃1주자 상황을 만듦 => 타자의 Run Value = 0.913 - 0.498 = 0.415
* 각 팀의 종합 Run Value가 승률에 얼마나 영향을 미쳤는지 분석한다.

<br/>  
<br/>

## 파워형 투수 vs 기교파 투수

### Description

* 파워형 투수(Power Pitcher)와 기교파 투수(Finesse Pitcher) 유형별 성적 특징 분석.

### 경기 기록 데이터 분석

* [Power Vs Finesse](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_Pitcher_Data(Power_vs_Finesse).ipynb)

### 분석

* PFR 수치를 계산하여 투수를 파워형과 기교파로 분류 [ PFR = ( K + BB ) / IP ]
* PFR 수치 상위 25%(Power)와 하위 25%(Finesse)를 기록한 투수들의 성적 비교

<br/>   
<br/>

## 류현진 투수 투구 데이터 분석

### Description

* 류현진 선수의 투구 데이터 시각화 및 분석.

### 류현진 투구 데이터 분석

* [Ryu_Pitch](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_Ryu_pitch_data_2019.ipynb)

### 분석

* 류현진 선수의 구종 구사 비율 분석.
* 구사 비율이 가장 높은 FF(포심), CH(체인지업)을 MLB 평균 데이터와 비교 분석.
* 투구 결과를 시각화.
* 류현진 선수가 선발 등판한 경기 별 투구 수와 가장 공을 많이 던지게 한 상대 타자 분석.
* 아웃 종류(삼진, 땅볼, 플라이)별 구종 비교 분석.

<br/>
<br/>

## BABIP 데이터 분석

### Description

* Batting Average on Balls in Play (BABIP) 분석

### 리그 전체 타자들의 BABIP 연도별 변화 분석

* [BABIP](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_BABIP_batter.ipynb)

### 분석

* 홈런이 아닌 타구가 얼마나 in play 되는가를 나타내는 비율.
* BABIP 수치에는 '운'도 따르기 때문에 많은 Sample size가 필요.
* 연도별 리그 전체 BABIP이 어떻게 변화했는지 시각화.
* BABIP수치는 평균적으로 0.3에 근사.

<br/>
<br/>

## MONEY BALL 분석

### Description

* 장타율 VS 출루율 분석

### 장타율과 출루율 중 어느 지표가 더 승률에 영향을 미치는지 분석

* [Moneyball](https://github.com/pcw789/sports_analysis_python/blob/main/MLB_moneyball_practice.ipynb)

### 분석

* 99시즌~02시즌 각 팀의 승률, 장타율, 출루율 계산
* 승률(독립변수), 장타율과 출루율(종속변수)로 선형 회귀 분석 수행
* 장타율과 승률과의 관계, 출루율과 승률과의 관계 분석

<br/>
<br/>

## FF(포심패스트볼) 분석

### Description

* 21년 메이저리그 포심패스트볼 데이터 분석

### 포심패스트볼의 구속, 회전수, 피안타율, 타구 속도 관계 분석

* [FF_data](https://github.com/pcw789/sports_analysis_python/blob/main/FF_data.ipynb)

### 분석

* 공의 회전수와 구속의 관계 분석
* 공의 회전수와 피안타율의 관계 분석
* 공의 구속과 타구 속도와의 관계 분석

