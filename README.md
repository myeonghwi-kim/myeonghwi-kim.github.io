# Myeonghwi-Kim Portfolio

### 예측기 실행 방법
- model.py 파일의 load_model 함수 실행 -> 모델 생성 및 저장
- load_model의 파라미터는 업데이트마다 모델을 저장시키기위한 역할 -> 기본은 NONE

### Web Service 실행 방법
- 기본 URL 요청시 cvr.html로 이동(렌더링)
- prediction 메소드 : 클라이언트에서 Test Dataset을 입력하면 데이터 포맷팅->  cvr.html로 리턴 후 렌더링
- update 메소드 : 클라이언트에서 업데이트를 요청 -> cvt.html로 리턴 후 load_model 함수 실행(파라미터는 초기와 구분을 위해 Temp 입력)
- main : 서버 시작 시 기존 학습 모델 로드, Flask 서버 기동

### 분석 결과
- 평가 지표 : Accuracy, Precision, Recall, F1-Score


|평가지표|학습데이터|평가데이터|
|:--:|:--:|:--:|
|Accuracy|1.000|1.000|
|Precision|1.000|1.000|
|Recall|0.997|0.997|
|F1-Score|0.998|0.998|


### 분석

![슬라이드1](https://user-images.githubusercontent.com/74284500/116784388-eeb8b780-aace-11eb-89d2-9da6cd24ae74.JPG)
