# ESP8266-smart-alarm-webserver
![](https://github.com/siz0001/ESP8266-smart-alarm-webclient/blob/master/src/assets/schematics.png)
- ESP8266 를 웹 서버로 만들고, 
- Ultrasonic Sensor(HC-SR04)를 통해 받은 거리값의 변화를 통해 
- 엘리베이터 문이 열리고 손님이 입장하는 것을 감지후 
- 거리값을 REST API로 송신하는 시스템

## router 세팅
- 제조사의 라우터 옵션 설정에서 ESP8266의 접속 IP를 내부 IP로 고정(iptime의 경우 192.168.0.1 혹은 192.168.1.1 에 접속후 수동 ip설정에서 수정)
- server IP 기본값은 192.169.1.200 이나, 이미 사용하고 있어 다른 IP를 사용해야 할 경우  store/index.js 에서 수정 가능

## cable connect
- 도선 연결은 매우 간단함. HC-SR04의 trig = D4, echo = D2에 연결하면 됨
  
<a href="https://github.com/siz0001/ESP8266-smart-alarm-webclient"></a> 에서 client 파일 참조
