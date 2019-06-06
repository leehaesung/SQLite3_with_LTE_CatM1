## 주피터 노트북(파이썬)에서 실시간 온도 데이타를 SQL에 저장하고 시계열분석

## 1. 셋팅하기

***

![image01](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/01_Setting.png)

***

## 2. 아루두이노 .ino 파일 업로드하기

- [.ino 파일: f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino ](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/02_Codes/f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino)
- 업로드끝나면 CatM1 보드의 오른쪽 전원(SW1 PWRKEY)을 켜주고 시리얼모니터에서 온도 데이타가 나오는지 확인합니다.

***

## 3. 데이타 분석
##### 전통적인 시계열 분석, 딥러닝 분석(RNN, LSTM)

- [Jupyter Web Viewer](https://nbviewer.jupyter.org/github/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.4.ipynb)  (주의! 스크롤링 압박이 올수 있음)
- [Jupyter notebook](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.4.ipynb)

- [Data sets: temp_catm1.csv](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/03_DataSets/temp_catm1.csv)

![image07](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_5.png)
![image04](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_2.png)
![image05](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_3.png)
![image06](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_4.png)
![image06](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_6.png)
![image07](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/Figure_1.png)

***

# References
- [GitHub: WIZNet IoT shield arduino](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr)
- [How to Install SQLite On Windows/ Linux / Mac OS X](http://www.codebind.com/sqlite/how-to-install-sqlite-on/)
- [SQLite Tutorial](https://www.tutorialspoint.com/sqlite/)
- [SQLite Quick Guide](https://www.tutorialspoint.com/sqlite/sqlite_quick_guide.htm)
- [SQLite - Python Tuotorial](https://www.tutorialspoint.com/sqlite/sqlite_python.htm)
- [SQLite - Python Quick Guide](https://github.com/leehaesung/SQLite-Python_Quick_Guide)
