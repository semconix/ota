
ESP32 → STM32 OTA Test Repository

Structure:
firmware/stm32_v1.0.1.bin   - Example firmware binary
version.json                - OTA metadata file

Typical OTA Flow:
1. ESP32 downloads version.json
2. Compares device firmware version
3. If newer version available
4. ESP32 downloads firmware binary
5. Sends firmware to STM32 bootloader over UART
