## 주피터 노트북(파이썬)에서 온도 데이타를 SQL에 저장하고 시계열분석

## 1. 셋팅하기

***

![image01](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/01_Setting.png)

***

## 2. 아루두이노 .ino 파일 업로드하기

- [.ino 파일: f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino ](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/02_Codes/f_WIoT-QC01_Arduino_MQTT_SEND_JSON.ino)
- 업로드끝나면 CatM1 보드의 오른쪽 전원(SW1 PWRKEY)을 켜주고 시리얼모니터에서 온도 데이타가 나오는지 확인합니다.

***

## 3. 데이타분석

![image02](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/03_Jupyter_notebook.png)
![image03](https://raw.githubusercontent.com/leehaesung/SQLite3_with_LTE_CatM1/master/01_Images/02_Jupyter_notebook.png)

- [Jupyter Web Viewer](https://nbviewer.jupyter.org/github/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.3.ipynb)
- [Jupyter notebook](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/blob/master/02_Codes/SQLite3_with_LTE_CatM1_Temp_Sensor_MQTT_VER_0.3.ipynb)

- [Data sets: temp_catm1.csv](https://github.com/leehaesung/SQLite3_with_LTE_CatM1/raw/master/03_DataSets/temp_catm1.csv)

***

# References
- [GitHub: WIZNet IoT shield arduino](https://github.com/Wiznet/wiznet-iot-shield-arduino-kr)
- [How to Install SQLite On Windows/ Linux / Mac OS X](http://www.codebind.com/sqlite/how-to-install-sqlite-on/)
- [SQLite Tutorial](https://www.tutorialspoint.com/sqlite/)
- [SQLite Quick Guide](https://www.tutorialspoint.com/sqlite/sqlite_quick_guide.htm)
- [SQLite - Python Tuotorial](https://www.tutorialspoint.com/sqlite/sqlite_python.htm)
- [SQLite - Python Quick Guide](https://github.com/leehaesung/SQLite-Python_Quick_Guide)
