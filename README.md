# STM32F1 (http://wiki.stm32duino.com/index.php?title=Blue_Pill) Radio Control USB adapter for Turnigy 9x, OpenTX 14CH PPMSim.

Allows Turnigy 9x with OpenTX firmware to connecto a PC as a USB HID game controller.
All switches, knobs, and sticks are activated.

Based on same project for STM32F3Discovery: https://github.com/alexeystn/stm32-ppm-usb-adapter, but ported for STM32F1 (tested on STM32F103C8) controllers.

Project for CooCox IDE.

Compiled binaries can be found in Debug dir: https://github.com/shaiku/STM32-RC-USB-Adapter/tree/master/stm32_PPM_F103/Debug/bin

#Connections:
- RC PPM out <==> PA8
- RC GND <==> GND

#Transmitter Configuration
Load OpenTX firmware for 9x: https://www.open-tx.org/

* Create a new model for the simulator
* On the SETUP page, change Proto to PPMSim 14CH
* On the MIXER page configure channels
    * CH1:  Rud
    * CH2:  Ele
    * CH3:  Thr
    * CH4:  Ail
    * CH5:  P1
    * CH6:  P2
    * CH7:  P3
    * CH8:  3POS
    * CH9:  THR
    * CH10: RUD
    * CH11: ELE
    * CH12: AIL
    * CH13: GEA
    * CH14: TRN