# Especificaciones del Proyecto: CM4 Robotics Controller (Versión Limpia)

Este documento detalla las especificaciones de diseño para la placa de control robótico basada en Raspberry Pi Compute Module 4 (CM4), con enfoque en la integración de conectividad USB Tipo-C y almacenamiento NVMe.

## 1. Visión General del Proyecto

El objetivo de este proyecto es desarrollar una placa portadora compacta y versátil para el Raspberry Pi CM4, diseñada para aplicaciones robóticas y de automatización. La placa proporcionará interfaces esenciales para la comunicación, alimentación y control de periféricos, incluyendo soporte para una cámara OAK-D-Lite y almacenamiento de alta velocidad.

## 2. Componentes Principales

*   **Raspberry Pi Compute Module 4 (CM4)**: El cerebro de la placa, proporcionando capacidad de procesamiento y conectividad.
*   **Conector USB Tipo-C**: Para alimentación y comunicación de datos de alta velocidad con el CM4.
*   **Conector M.2 (Key M)**: Para la integración de un disco de estado sólido NVMe, ofreciendo almacenamiento de alta velocidad.
*   **Conectores para subsistemas**: Interfaces para subsistemas de alimentación, control de motores, sensores y otros periféricos.

## 3. Requisitos de Conectividad

### 3.1. USB Tipo-C

*   **Funcionalidad**: Soporte para alimentación (Power Delivery si es posible, o al menos 5V) y datos USB 2.0/3.0.
*   **Integración**: Conexión directa al CM4 para aprovechar su capacidad USB.

### 3.2. NVMe (PCIe)

*   **Funcionalidad**: Interfaz PCIe Gen 2 x1 para un disco SSD M.2 NVMe.
*   **Formato**: Soporte para módulos M.2 2230/2242/2260/2280.

### 3.3. OAK-D-Lite

*   **Comunicación**: Conectividad USB 3.0 (SuperSpeed) a través del conector USB Tipo-C.
*   **Alimentación**: Suministro de energía adecuado para la cámara a través del mismo conector.

## 4. Requisitos de Alimentación

*   **Entrada de Alimentación**: Rango de voltaje de entrada amplio (ej. 7V-24V) para flexibilidad en aplicaciones robóticas.
*   **Reguladores de Voltaje**: Generación de voltajes estables de 5V y 3.3V para el CM4 y periféricos.
*   **Protección**: Protección contra sobrecorriente, sobrevoltaje y polaridad inversa.

## 5. Requisitos de Diseño de PCB

*   **Dimensiones**: Compactas para adaptarse a chasis robóticos.
*   **Capas**: Mínimo 4 capas para un enrutamiento eficiente y control de impedancia para señales de alta velocidad (USB 3.0, PCIe).
*   **Señales de Alta Velocidad**: Enrutamiento diferencial para USB 3.0 y PCIe, con control de impedancia y longitud de traza.
*   **Disipación de Calor**: Consideraciones para la disipación de calor del CM4 y otros componentes de potencia.
*   **Conectores**: Selección de conectores robustos y fiables para entornos robóticos.

## 6. Control de Versiones

*   **Sistema**: Git.
*   **Ramas**: `main` para la versión estable, `develop` para el desarrollo activo, y ramas de características para nuevas funcionalidades.

## 7. Documentación

*   **Esquemáticos**: Archivos `.kicad_sch` para cada subsistema y el esquemático principal.
*   **Layout de PCB**: Archivo `.kicad_pcb`.
*   **Bibliotecas**: Archivos `.kicad_sym` y `.kicad_mod` para símbolos y footprints personalizados.
*   **Archivos de Fabricación**: Generación de archivos Gerber, drill files, BOM, y Pick and Place.
*   **README.md**: Descripción general del proyecto y guía de inicio rápido.
*   **kicad_cli_tutorial.md**: Tutorial para la automatización del diseño de PCB con KiCad CLI.

