# Remote ID Module for Drones using ESP32 and ArduRemoteID

This project demonstrates a cost-effective implementation of a Remote ID system for drones, using the ESP32-S3 microcontroller and ArduRemoteID firmware. It is fully compatible with ArduPilot-based flight controllers (e.g., Cube Orange) and satisfies FAA Remote ID requirements.

## 📦 Features
- Uses ESP32-S3 for Wi-Fi-based Remote ID broadcasting
- Compatible with Cube Orange & Here4 GPS
- Broadcasts location using UART protocol (ODID standard)
- Real-time data visible in OpenDroneID app
- Low-cost alternative (under \$30)

## 🛠 Hardware Used
- ESP32-S3 module
- Cube Orange (with ArduPilot firmware)
- Here4 GPS
- Optional: power distribution board, telemetry radio

## 📁 Folder Overview
- `docs/`: Final report, diagrams, and explanation PDFs
- `firmware/`: Precompiled binary for ESP32 RemoteID
- `hardware/`: Wiring diagrams and notes
- `src/`: Example code and data parsing scripts
- `references/`: BibTeX references used in documentation
- `images/`: Setup and result screenshots

## 📷 System Architecture
![System Diagram](images/architecture_diagram.png)

## 🧠 Methodology Summary
1. Flashed `ArduRemoteID.bin` to ESP32-S3
2. Compiled Cube Orange firmware with ODID support
3. Connected ESP32 to flight controller via UART
4. Verified output on OpenDroneID app

## 📊 Results
- Accuracy: ~25 cm
- Latency: 10 ms
- Broadcast Protocol: Wi-Fi (preferred over BLE)

## 🔗 Useful Links
- [ArduPilot Remote ID Docs](https://ardupilot.org/copter/docs/common-remoteid.html)
- [ArduRemoteID GitHub](https://github.com/ArduPilot/ArduRemoteID)
- [OpenDroneID](https://opendroneid.org)

## 📜 License
[MIT License](LICENSE)

---

Feel free to fork, modify, or improve this project.
