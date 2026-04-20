# integrated-soundlevelmeter-dosimeter
Integrated Sound Level Meter and Dosimeter — ESP32 + INMP441 + ILI9341 TFT
# Integrated Sound Level Meter and Dosimeter

A low-cost integrated occupational noise monitoring device combining 
a Sound Level Meter, Noise Dosimeter, and 9-band Octave Analyser 
on a single ESP32 platform.

## Features
- Real-time A-weighted SPL (dB(A)) — IEC 61672-1
- OSHA dosimetry — dose%, TWA, 5 dB exchange rate
- 9-band octave spectrum — 31.5 Hz to 8 kHz, IEC 61260-1
- ILI9341 2.4" TFT colour display — 3 screens
- WiFi dashboard at http://192.168.4.1
- Session storage (last 5 sessions in NVS flash)
- ±1 dB(A) accuracy validated against B&K Class 1 SLM

## Hardware
- ESP32 DevKit V1
- INMP441 I2S MEMS microphone
- ILI9341 2.4" TFT SPI display (SBT240-W61 V01)

## Credits
The DSP core (I2S reader, MIC_EQ filter, A-weighting IIR cascade, 
and SPL formula) is based on the excellent work by **Ikostoski**:

> esp32-i2s-slm — https://github.com/ikostoski/esp32-i2s-slm  
> Copyright (c) 2020 Ikostoski — MIT License

## License
MIT License — see LICENSE file
