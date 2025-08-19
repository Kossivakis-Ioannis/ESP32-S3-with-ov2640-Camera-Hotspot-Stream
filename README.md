# ESP32-S3 Camera Hotspot Stream

This project allows you to **connect directly to an ESP32-S3 camera** via its own Wi-Fi hotspot and view a **live video stream**. The onboard LED will light up whenever motion is detected.

## Features
- **Direct hotspot connection** — no external Wi-Fi needed.
- **Live video stream** viewable on your phone or computer.
- **Onboard LED (GPIO2)** lights up on motion detection.
- Fully **portable** — just power the ESP32-S3 and connect.

## Hotspot Details
- **Hotspot Name (SSID):** `ESP32_CAM_AP`
- **Password:** `12345678`

> You can change the hotspot name and password in the code if desired.

## How to Connect
1. Power your ESP32-S3 board.
2. On your phone or computer, search for Wi-Fi networks.
3. Connect to the hotspot:
   - **SSID:** `ESP32_CAM_AP`
   - **Password:** `12345678`
4. Open a web browser and enter the IP address: `http://192.168.4.1/`
5. You will see the live video stream. The LED will light up when motion is detected.

## Customization
- **Change Hotspot credentials**:

```cpp
const char* ssid = "Your_Hotspot_Name";
const char* password = "Your_Password";
