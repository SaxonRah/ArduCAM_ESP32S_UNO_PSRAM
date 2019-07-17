# ArduCAM_ESP32S_UNO_PSRAM

## Development Status
Most of the framework is implemented. Most noticeable is the missing analogWrite. While analogWrite is on it's way, there are a few other options that you can use:
- 16 channels [LEDC](cores/esp32/esp32-hal-ledc.h) which is PWM
- 8 channels [SigmaDelta](cores/esp32/esp32-hal-sigmadelta.h) which uses SigmaDelta modulation
- 2 channels [DAC](cores/esp32/esp32-hal-dac.h) which gives real analog output

## Installation Instructions
- Using Arduino IDE Boards Manager (preferred)
  + [Instructions for Boards Manager](docs/arduino-ide/boards_manager.md)
- [Using OTAWebUpdater](docs/OTAWebUpdate/OTAWebUpdate.md)

#### Issue/Bug report template
Before reporting an issue, make sure you've searched for similar one that was already created. Also make sure to go through all the issues labelled as [for reference](https://github.com/espressif/arduino-esp32/issues?utf8=%E2%9C%93&q=is%3Aissue%20label%3A%22for%20reference%22%20).

Finally, if you're sure no one else had the issue, follow the [ISSUE_TEMPLATE](docs/ISSUE_TEMPLATE.md) while reporting any issue.

## ArduCAM_ESP32S_UNO_PSRAM Board PINMAP

![Pin Functions](docs/esp32_pinmap.png)

## Hint

Sometimes to program ESP32 via serial you must keep GPIO0 LOW during the programming process
