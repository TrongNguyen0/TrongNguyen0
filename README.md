<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=wave&color=0:0F172A,100:1E40AF&height=240&section=header&text=Tr%E1%BA%A7n%20Tr%E1%BB%8Dng%20Nguy%C3%AAn&fontColor=F1F5F9&fontSize=44&fontAlignY=26&desc=Embedded%20Systems%20%C2%B7%20IoT%20%C2%B7%20TinyML&descSize=18&descAlignY=44&animation=fadeIn" width="100%" alt="Trần Trọng Nguyên · Embedded Systems · IoT · TinyML"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=800&color=3B82F6&center=true&vCenter=true&width=560&lines=Firmware+for+ESP32-S3+%26+STM32;Secure+OTA%3A+signed%2C+delta%2C+rollback;TinyML+on+microcontrollers;Linux+servers+on+Raspberry+Pi+5" alt="Firmware for ESP32-S3 & STM32 · Secure OTA · TinyML · Raspberry Pi servers"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Open%20to-internship-2563EB?style=for-the-badge&labelColor=0F172A" alt="Open to internship"/>
  <a href="mailto:nguyen28yn@gmail.com"><img src="https://img.shields.io/badge/Email-nguyen28yn%40gmail.com-1E3A8A?style=for-the-badge&labelColor=0F172A&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://www.facebook.com/trongnguyendz"><img src="https://img.shields.io/badge/Facebook-trongnguyendz-1E3A8A?style=for-the-badge&labelColor=0F172A&logo=facebook&logoColor=white" alt="Facebook"/></a>
</p>

## 👋 About me

Embedded systems student who enjoys the whole path from a sensor register to a server dashboard.

- 🔧 Firmware for **ESP32-S3** (ESP-IDF) and **STM32** (Zephyr + MCUboot)
- 🔐 Secure firmware updates: signed manifests, delta patches, A/B slots, rollback, Secure Boot
- 🧠 TinyML: int8 models running on the microcontroller with TensorFlow Lite Micro
- 🖥️ Self-hosted Linux servers on Raspberry Pi 5 with Docker, Caddy and Cloudflare Tunnel
- 🌱 Looking for an **internship** in embedded systems / IoT

> 🇻🇳 Xin chào! Mình là Nguyên, sinh viên theo hướng hệ thống nhúng và IoT: viết firmware cho ESP32/STM32,
> cập nhật OTA an toàn và chạy AI ngay trên vi điều khiển. Mình đang tìm cơ hội thực tập.

## 🛠️ Tech stack

<p>
  <img src="https://img.shields.io/badge/ESP32--S3-1E3A8A?style=flat-square&logo=espressif&logoColor=white" alt="ESP32-S3"/>
  <img src="https://img.shields.io/badge/STM32-1E3A8A?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32"/>
  <img src="https://img.shields.io/badge/ESP--IDF-1E3A8A?style=flat-square&logo=espressif&logoColor=white" alt="ESP-IDF"/>
  <img src="https://img.shields.io/badge/Zephyr%20RTOS-1E3A8A?style=flat-square" alt="Zephyr RTOS"/>
  <img src="https://img.shields.io/badge/MCUboot-1E3A8A?style=flat-square" alt="MCUboot"/>
  <img src="https://img.shields.io/badge/BLE-1E3A8A?style=flat-square&logo=bluetooth&logoColor=white" alt="BLE"/>
  <img src="https://img.shields.io/badge/TFLite%20Micro-1E3A8A?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow Lite Micro"/>
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=c,cpp,py,bash,linux,docker,raspberrypi,tensorflow,fastapi,sqlite,qt,cmake,git,githubactions&theme=dark"/>
  <img src="https://skillicons.dev/icons?i=c,cpp,py,bash,linux,docker,raspberrypi,tensorflow,fastapi,sqlite,qt,cmake,git,githubactions&theme=light" alt="C, C++, Python, Bash, Linux, Docker, Raspberry Pi, TensorFlow, FastAPI, SQLite, Qt, CMake, Git, GitHub Actions"/>
</picture>

## 🚀 Featured project

### 🔒 [secure-tinyml-ota](https://github.com/TrongNguyen0/secure-tinyml-ota) &nbsp;<sub>private · graduation thesis, in progress</sub>

Vibration monitoring with TinyML on ESP32-S3, plus secure over-the-air updates of both the firmware and the AI model,
served from a Raspberry Pi 5 ([pi-server](https://github.com/TrongNguyen0/pi-server)).

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/architecture-dark.svg"/>
  <img src="assets/architecture-light.svg" width="100%" alt="ADXL345 feeds an ESP32-S3 running TinyML; a Raspberry Pi 5 sends signed updates to it and receives telemetry; a phone updates it over BLE; it updates an STM32 node over UART (SMP)"/>
</picture>

- **On-device AI:** ADXL345 at 3.2 kHz → FFT features → int8 autoencoder + fault classifier, on-device calibration and drift detection
- **Update security:** CBOR/COSE (SUIT-style) signed manifests, anti-rollback, A/B model slots tested against power cuts, Secure Boot v2 + Flash Encryption
- **Delivery:** delta updates at ~2% of full size, BLE OTA, per-device signed requests, staged rollouts that halt themselves on failures
- **STM32 node:** Zephyr + MCUboot, updated through the ESP32-S3 over SMP
- **Testing:** 67k host checks under ASan/UBSan with fuzzing, end-to-end tests against the real server, CI

## 🐍 Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/TrongNguyen0/TrongNguyen0/output/github-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/TrongNguyen0/TrongNguyen0/output/github-snake.svg"/>
  <img alt="Contribution graph eaten by a snake" src="https://raw.githubusercontent.com/TrongNguyen0/TrongNguyen0/output/github-snake.svg"/>
</picture>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=wave&color=0:0F172A,100:1E40AF&height=110&section=footer" width="100%" alt=""/>
</p>
