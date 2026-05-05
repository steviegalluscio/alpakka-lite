# Alpakka Lite
## Wiring
| Pin | Destination | Notes |
| --- | --- | --- |
| GPIO 2 | Left IMU SCL (SCK)  |  |
| GPIO 3 | Left IMU SDA (MOSI) |  |
| GPIO 4 | Left IMU SAO (MISO) |  |
| GPIO 5 | Left IMU CS  |  |
| GPIO 6 | Touch OUT | Short to GPIO 7 via 100k ohm |
| GPIO 7 | Touch IN | Wire to thumbscrew   |
| GPIO 10 | Right IMU SCL (SCK)  |  |
| GPIO 11 | Right IMU SDA (MOSI) |  |
| GPIO 12 | Right IMU SAO (MISO) |  |
| GPIO 13 | Right IMU CS  |  |
| VBUS | USB 5V  |  Controller PCB  |
| VBUS | USB 5V (Red)  | Controller cable  |
| TP1 | USB GND (Black)| Controller cable  |
| TP2 | USB D- (White) | Controller cable  |
| TP3 | USB D+ (Green) | Controller cable  |
| 3V3 | Left IMU VIN   |  |
| 3V3 | Right IMU VIN  |  |
| GPIO 20 | USB D- | Controller PCB        |
| GPIO 21 | USB D+ | Controller PCB        |
| GND | USB GND | Controller PCB (2 pads, tie both to same or diff GND) |




See: https://github.com/steviegalluscio/alpakka_firmware/blob/88f42c9516ef7bdc2893ddaced1abc7dd2f941d2/src/headers/pin.h#L74-L131


TODO: add photo or diagram
