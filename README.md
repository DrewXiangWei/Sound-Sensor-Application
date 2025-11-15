# Sound-Sensor-Application
This project was target to link the raspberry pi with the android studio application in my phone to built up a real time noise monitoring systemwith raspberry pi + gpio mic-> Android live chart with TCP socket streaming.

Key Features
| Feature | Implementation |
|--------|----------------|
| **Real-time dB** | GPIO sound sensor → **moving average** in Python |
| **Live Android Chart** | **MPAndroidChart** + **TCP streaming** |
| **Historical Trends** | **SQLite** on Pi → export CSV |
| **User Interface** | Dark mode, decibel meter, alert thresholds |
| **Auto-reconnect** | Socket retry logic on Android |
#Raspberry Pi (server)
pip install -r requirements.txt
python3 server.py
#Android
Open Android Studio → Run `SoundMonitorApp` on device
#Setup Guide
Hardware
- Raspberry Pi 3/4/Zero W
- USB Microphone or GPIO sound sensor
- Android phone (API 21+)
Software
```bash
sudo apt install python3-pip git
git clone https://github.com/DrewXiangWei/Sound-Sensor-Application.git
cd Sound-Sensor-Application
pip install -r requirements.txt
