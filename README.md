# 서울시 따릉이 수요 조사 데이터 분석 및 시각화

# 컬럼 설명
- id 고유 id
- hour 시간
- temperature 기온
- precipitation 비가 오지 않았으면 0, 비가 오면 1
- windspeed 풍속(평균)
- humidity 습도
- visibility 시정(視程), 시계(視界)(특정 기상 상태에 따른 가시성을 의미)
- ozone 오존
- pm10 미세먼지(머리카락 굵기의 1/5에서 1/7 크기의 미세먼지)
- pm2.5 미세먼지(머리카락 굵기의 1/20에서 1/30 크기의 미세먼지)
- count 시간에 따른 따릉이 대여 수

## 분석
- 따릉이는 서울특별시에서 2014년부터 시범 운영을 시작하고 2015년 10월부터 본격적으로 정식 운영을 시행한 완전 무인 공공자전거 대여 서비스이다.
- 대중교통 이후의 환승으로 따릉이 사용이 가능하다.

1. **퇴근시 대중교통 이후에 따릉이 사용의 빈도 파악**
2. **퇴근 이후 한강 등 산책의 용도로 사용 빈도**
3. **온도에 따른 수요 분석**

## 상관분석 결과

- 시간과 온도 햇빛의 유무 양의 상관관계
- 온도와 습도에 대한 음의 상관관계
- 시간에 대한 오존 = 햇빛
- 온도/오존과 풍속의 관계
- 습도 가시성의 관계
- 습도와 오존에 대한 음의 상관관계
- 미세먼지와 가시성과의 관계

### 상관분석 결과에 따른 추측

1. 따릉이를 타는 시간은 출퇴근 시간에 수요가 많을 것이다.
2. 날씨가 너무 덥거나, 추운시간에는 수요가 적을 것이다.
3. 비가 오는 날(습도가 높은날)에는 수요가 적을 것이다.
4. 온도가 높은 날에는 오존이 높으며, 풍속도 빠를 것이다.
5. 습도가 높은 날에는 가시성이 낮을 것이며, 이에 따라 수요가 적을 것이다.
6. 미세먼지가 높은 날에는 수요가 적을 것이다.
