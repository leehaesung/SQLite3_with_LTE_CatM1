# Jupyter 노트북(Python)에서 실시간 온도 데이타를 SQL에 저장하고 시계열분석

## 1. WIZnet IoT Cat.M1 개발보드 정보

***

* SKT텔레콤 5G LTE Cat.M1은 [BG96 IoT통신모듈](https://www.sktiot.com/iot/introduction/network/networkCatM1Main5)이 내장된 [WIZnet](https://www.wiznet.io/ko/) 개발보드입니다.
* [WIZnet IoT shield 랜딩 페이지는](https://github.com/Wiznet/wiznet-iot-shield-kr) 다양한 하드웨어 플랫폼에서 활용 할 수 있는 예제 코드와 시작 가이드 및 어플리케이션 노트 등의 문서를 제공합니다.
* [WIZnet IoT shield 하드웨어 가이드[GitHub]](https://github.com/Wiznet/wiznet-iot-shield-kr)는 Pinout, layout, Schematic, Gerber, BOM 등 포함합니다.
* Arduino(아루두이노) WIZnet IoT 쉴드 플랫폼 개발 가이드 [[GitHub]](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr), [[Wiki문서]](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr/wiki), [[YouTube]](https://youtu.be/BCkNTRGBWxE)
* Raspberry Pi(라즈베리파이) WIZnet IoT 쉴드 플랫폼 개발 가이드 [[GitHub]](https://github.com/Wiznet/wiznet-iot-shield-raspberrypi-kr), [[Wiki문서]](https://github.com/Wiznet/wiznet-iot-shield-raspberrypi-kr/wiki), [[YouTube]](https://youtu.be/yERjOIvN7sE)
* Arm Mbed WIZnet IoT 쉴드 플랫폼 개발 가이드 [[GitHub]](https://github.com/Wiznet/wiznet-iot-shield-mbed-kr), [[Wiki문서]](https://github.com/Wiznet/wiznet-iot-shield-mbed-kr/wiki), [[YouTube]](https://youtu.be/bsrNez7uaf8)
* SKT텔레콤 5G LTE [Cat.M1/LTE-M 기본 IoT 요금제 리스트](https://www.sktiot.com/iot/introduction/paymentSystem/paymentSystemCatM1)입니다. 

## 2. 개발보드조립 및 점퍼셋팅하기

***

![image01](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/01_Setting.png)

***

## 3. 아루두이노 .ino 파일 업로드하기

- [.ino 파일: f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino(소스코드)[GitHub]](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/02_Codes/f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino)
- 업로드 하기전에 [Arduino 기반의 Cat.M1 MQTT 테스트 가이드[GitHub]](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr/blob/master/docs/Arduino_guide_qc-bg96_mqtt.md)를 습득하시기 바랍니다.
- 업로드끝나면 CatM1 보드의 오른쪽 전원(SW1 PWRKEY)을 켜주고 시리얼모니터에서 온도 데이타가 나오는지 확인합니다.

***

## 4. 데이타 분석
* WIZnet IoT 개발보드에 있는 디지탈 온도센서를 이용해서 사무실의 온도를 측정, 수집, SQL쿼리, 그리고 [케라스(딥러닝플랫폼)](https://keras.io/)로 분석합니다. 
* 전통적인 시계열 분석, 딥러닝 분석(RNN, LSTM)

- [Jupyter Web Viewer(소스코드)](https://nbviewer.jupyter.org/github/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.4.ipynb) 
- [Jupyter notebook(소스코드)](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.4.ipynb)

- [Data sets: temp_catm1.csv(온도 데이타셋)](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/03_DataSets/temp_catm1.csv)

![image07](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_5.png)
![image04](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_2.png)
![image05](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_3.png)
![image06](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_4.png)
![image06](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_6.png)
![image07](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_1.png)
![image08](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_7.png)

***

# 5. References
- [GitHub: WIZNet IoT shield arduino](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr)
- [How to Install SQLite On Windows/ Linux / Mac OS X](http://www.codebind.com/sqlite/how-to-install-sqlite-on/)
- [SQLite Tutorial](https://www.tutorialspoint.com/sqlite/)
- [SQLite Quick Guide](https://www.tutorialspoint.com/sqlite/sqlite_quick_guide.htm)
- [SQLite - Python Tuotorial](https://www.tutorialspoint.com/sqlite/sqlite_python.htm)
- [SQLite - Python Quick Guide](https://github.com/leehaesung/SQLite-Python_Quick_Guide)
