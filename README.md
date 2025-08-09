Quick interactive demo: an ESP32 + HC-SR04 ultrasonic sensor sends distance readings to a Raspberry Pi Zero 2 W over Wi‑Fi. The Pi hosts a simple web page that visualizes distance with an animated orb. Designed for a 40-minute rapid-prototyping classroom session.

Contents:
1) esp32-firmware: ESP32 sketch and Wi‑Fi config template
2) raspberry-pi-server: Flask server + HTML/JS front-end
3) teaching-material: lesson plan, exercises, wiring guide

Hardware:
1) ESP32 development board
2) HC‑SR04 ultrasonic sensor
3) Raspberry Pi Zero 2 W with display, keyboard, mouse
4) Breadboard, jumper wires, resistor (for level shifting), power supply

Quick start

1) On Pi:
- Install Python 3 and pip, then: pip3 install -r requirements.txt
- Run: python3 app.py
  
2) On ESP32:
- Edit wifi_credentials.h with SSID, password, and Pi IP
- Flash ESP32_HCSR04_WIFI_POST.ino

3) In Pi browser: open http://<PI_IP>:5000/
