# ROBO CONTROL Premium — Android source
Open this folder in Android Studio and build the APK, or upload it to GitHub and use the included Actions workflow.

Features: Bluetooth Classic paired-device connection, F/B/L/R/S/X drive commands, speed command V0–V255, servo panel, mode panel, and ESP32-CAM MJPEG viewer.

IMPORTANT: Drive commands F/B/L/R/S/X are retained. Servo commands (`LH_UP`, `LH_DOWN`, `RH_UP`, `RH_DOWN`, `HEAD_LEFT`, `HEAD_RIGHT`, `HEAD_CENTER`) and mode commands (`MODE:<NAME>`) are template command strings. Match these to your existing ESP32 firmware parser before using those buttons. This source does not claim to know your firmware's exact servo/mode command strings.

Camera: enter the stream URL configured in your ESP32-CAM firmware. A common endpoint is `http://CAMERA_IP:81/stream`. Live video requires ESP32-CAM hardware, streaming firmware, and network connectivity.

No LED or MPU-6050 controls are included.
