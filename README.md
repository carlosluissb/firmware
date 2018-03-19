# Firmware

## Descripción

El siguiente repositorio contiene toda la implementación del firmware del proyecto Laser Tag. Se encarga de adquirir la data analogica y digital les aplica el protocolo de comunicaciones para enviarla via serial a ala computadora. 

## Table of Contents
- [Lista de Módulos](#lista-de-módulos)
- [Requisitos](#requisitos)
- [Software](#software)
- [License](#license)

## Lista de Módulos
- [Protocolo de Comunicaciones](https://github.com/Fedora-Eugenio/firmware/blob/master/CL1/Sources/main.c) Implementación de 4 canales de adquisición. Con capacidad para 8 sensores digitales y 4 analógicos. Se forman 4 canales mixtos cada uno de los cuales esta dividio en 2 mitades de 8 bits cada uno y una etiqueta al inicio de los 4 canales de la sigiente manera:
0xFN 0DDAAAAA 0AAAAAAA
#N: Nro. Canales Mixtos
#Dx: Sensor Digital
#Ax: Sensor Analógico
- [Events.h](https://github.com/Fedora-Eugenio/firmware/blob/master/CL1/Sources/Events.h) Módulo de eventos de Processor Expert.
- [Events.c](https://github.com/Fedora-Eugenio/firmware/blob/master/CL1/Sources/Events.c) Automatic Contrast-Limited AHE (CLAHE)

## Requisitos

La siguiente implementación fue desarrollada y probada en Windows 10 - 64 bits y Windows 7

## Software

- Implementación hecha en CodeWarrior v10.6 + Processor Expert.

## License

Copyright (c) 2017-2018 Fedora Di Polo - Eugenio Martínez
Released under the [GNU GPLv3.0 License](LICENSE). 
