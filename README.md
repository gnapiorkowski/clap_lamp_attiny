# Programming Attiny13

Arduino|Attiny13
-|-
D10|(Reset)
D11|(MOSI)
D12|(MISO)
D13|(SCK)
+5V| VCC
![Attiny13 pinout](https://camo.githubusercontent.com/f53f0c04f052aab3fddf233c6236154a1ee39ea4b64efe6ff1b1fc43f77cc52c/687474703a2f2f692e696d6775722e636f6d2f4a7362677550562e6a7067)

## Arduiono UNO
Attiny13 doesn't have serial, so programming is with Arduiono.

1. Arduiono IDE -> Example Arduino ISP
2. Upload to Arduino UNO


## ArduinoIDE Flashing Attiny13

1. Use framework for BoardSupport [MicroCroe](https://github.com/MCUdude/MicroCore)
2. use Attiny13 board
3. Burn Bootloader
4. Power cycle Attiny13
5. Upload sketch

## Platformio Flashing Attiny13

Project was set up with
`pio project init --board attiny13`

To flash Attiny13
`pio run --target upload`

It should automatically detect Arduino as ISP at /dev/ttyUSB<X>
and flash with no problems
