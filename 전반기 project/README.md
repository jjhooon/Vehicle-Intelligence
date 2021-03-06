# 차량지능기초 전반기 project #

구글의 미디어파이프 솔루션을 이용하여 차량지능 관련 주제의 간단한 프로젝트를 수행하였습니다.

### 문제 정의 ###

최근, 미국에서 테슬라 자율주행 기능인 '오토파일럿'을 오용하여 두 명이 사망하는 사고가 발생하였습니다. 

![image](https://user-images.githubusercontent.com/81551992/117570740-97d26400-b106-11eb-951b-41f908176b87.png)

이 사고의 원인을 바탕으로 **운전자의 실시간 검출**과 더불어 **졸음 운전을 감지하는 운전자 모니터링 시스템**을 만들었습니다.

### 미디어 파이프의 이용 ###

미디어파이프 솔루션 Face Detection과 Face Mesth를 합쳐 코드를 구현하였습니다.

Face Detection을 통하여 운전자의 존재 유무를 실시간으로 알 수 있고, Face Mesh의 Landmark 중 눈과 입에 해당하는 point를 추출하여 눈이 감기거나 하품을 하는 상황을 인식할 수 있었다.

### 결과 ###

![image](https://user-images.githubusercontent.com/81551992/117571329-13cdab80-b109-11eb-8220-0c3f8b44de23.png)
< Calibration 모드 >

![image](https://user-images.githubusercontent.com/81551992/117571613-41ffbb00-b10a-11eb-9306-934600102414.png)
< 운전자 상태 모니터링 모드 >

Calibration 모드를 통하여 기준을 얻고, 이를 바탕으로 운전자의 존재 유무와 졸음 운전을 실시간으로 인식한 것을 확인할 수 있습니다.

또한, LSTM 모델을 이용하여 운전자의 상태를 미리 예측할 수 있었습니다.

자세한 코드는 github을 통해 확인할 수 있으며 발표 영상 링크는 https://youtu.be/dSem0L04CFg 입니다.


