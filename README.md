# ESP32-Arduino-Servo-Library [![Build Status](https://travis-ci.org/RoboticsBrno/ESP32-Arduino-Servo-Library.svg?branch=master)](https://travis-ci.org/RoboticsBrno/ESP32-Arduino-Servo-Library)

Generate RC servo signal on a selected pin.

Base on [servo library for stm32f4 (d2a4a47)](https://github.com/arduino-libraries/Servo/blob/master/src/stm32f4/ServoTimers.h).

## Interface

The interface is similar to Arduino/Servo: https://www.arduino.cc/en/Reference/Servo

But the function `atach()` is different:

```c
bool attach(
    int pin,
    int channel = CHANNEL_NOT_ATTACHED,
    int minAngle = MIN_ANGLE,
    int maxAngle = MAX_ANGLE,
    int minPulseWidth = MIN_PULSE_WIDTH,
    int maxPulseWidth = MAX_PULSE_WIDTH
);
```

More information in [source code documentation](https://github.com/RoboticsBrno/ESP32-Arduino-Servo-Library/blob/master/src/Servo.h#L73).

Example: [04-SimpleServoAngles](examples/04-SimpleServoAngles/04-SimpleServoAngles.ino)

## PlatformIO

This library is also available at the [PlatformIO](https://platformio.org) as [ServoESP32](http://platformio.org/lib/show/1739/ServoESP32).