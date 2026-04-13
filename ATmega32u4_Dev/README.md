# ATmega32U4 Development Board

A custom development board based on the **ATmega32U4** microcontroller, designed for USB-enabled embedded projects, rapid prototyping, and firmware experimentation. This is a trial project to become familair with circuit and PCB design as well as serve as a base for future project prototyping.

## Overview

This project provides a hardware platform built around the ATmega32U4, a microcontroller with native USB support.

This makes it ideal for:

* USB HID devices (keyboards, mice, gamepads)
* Serial communication over USB (CDC)
* Custom USB devices
* General embedded applications

## Features

* ATmega32U4 microcontroller
* Native USB support (no external USB-to-UART chip required)
* On-board 5V voltage regulation
* Power and Dataline surge protection
* ISP programming header
* Power Status LED
* Programable on board LED (Pin 13)
* GPIO breakout pins
* 16MHz Crystal Oscillator
* Designed to fit standard breadboards

## Microcontroller Details

* **Core:** AVR 8-bit
* **Flash Memory:** 32 KB
* **SRAM:** 2.5 KB
* **EEPROM:** 1 KB
* **Clock Speed:**  16 MHz
* **Interfaces:**

  * USB 2.0 Full Speed
  * UART
  * SPI
  * I2C (TWI)

## Pinout

*Pinout has some to be desired. Future works will better address pin layout*

![](Images\PinOut.png)
