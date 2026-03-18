# Future Frame LightCore

Future Frame LightCore is a high precision illumination system designed for photographic film scanning. The device provides controlled multi channel lighting to ensure accurate color reproduction, uniform illumination, and additional imaging capabilities such as infrared dust detection.

## Overview

LightCore generates stable, controllable illumination using five independent light channels: red, green, blue, white, and infrared. The system allows precise control of light intensity and color balance, making it suitable for high quality digitization of photographic film.

A custom PCB and microcontroller system manage power delivery, LED current control, and system monitoring. 

## Hardware Architecture

The system is controlled by a Seeed Studio XIAO microcontroller mounted on a custom PCB. Power is delivered through a two stage regulation system that converts a high voltage input to stable low voltage rails for the electronics.

Key hardware components include:

* Seeed Studio XIAO microcontroller
* Four AL8860WT LED drivers
* Four channel DAC for current control
* MOSFET driver circuit for the infrared channel
* Temperature sensor for thermal monitoring

The LED drivers provide independent current control for the RGBW channels, while the infrared channel is used for dust detection and infrared transmission during scanning. 

## Power System

The board uses a two stage power conversion architecture:

* Buck converter: 36V to 5V
* LDO regulator: 5V to 3.3V

This configuration allows efficient power delivery while maintaining stable logic and control voltages. 

## Mechanical Design

The light source is mounted inside a custom enclosure consisting of:

* 3D printed structural housing
* Sheet aluminum side panels for rigidity
* Waterjet aluminum heat dissipator for thermal management
* Two stage diffusion system for uniform backlighting

A secondary control PCB inside the enclosure includes a rotary encoder, switches, and an OLED display for user interaction. 

## Features

* Five channel LED illumination system (RGB, white, infrared)
* High precision current control
* Active temperature monitoring
* Uniform diffused backlighting
* Integrated user control interface


