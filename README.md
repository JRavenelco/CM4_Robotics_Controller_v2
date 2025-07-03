# CM4 Robotics Controller - Clean Version

Este es un proyecto de KiCad para un controlador robótico basado en el Raspberry Pi Compute Module 4 (CM4), con soporte para USB Tipo-C y NVMe.

## Estructura del Proyecto

- `CM4_Robotics_Controller_Clean.kicad_pro`: Archivo principal del proyecto KiCad.
- `CM4_Robotics_Controller_Clean.kicad_sch`: Esquemático principal.
- `CM4_Robotics_Controller_Clean.kicad_pcb`: Layout de la placa de circuito impreso.
- `schematics/`: Contiene los esquemáticos jerárquicos de los subsistemas.
  - `Power_Subsystem.kicad_sch`: Subsistema de alimentación.
  - `CM4_Subsystem.kicad_sch`: Subsistema del CM4.
  - `RP2040_Subsystem.kicad_sch`: Subsistema del RP2040.
  - `Motor_Driver_Subsystem.kicad_sch`: Subsistema de drivers de motor.
  - `Sensor_Subsystem.kicad_sch`: Subsistema de sensores.
  - `USB_Subsystem_V2.kicad_sch`: Subsistema USB con conector Tipo-C.
  - `PCIe_NVMe_Subsystem.kicad_sch`: Subsistema PCIe para NVMe.
- `lib_symbols/custom/`: Librerías de símbolos esquemáticos personalizados.
- `lib_footprints/custom/`: Librerías de footprints personalizados.

## Características Clave

- **Raspberry Pi Compute Module 4 (CM4)**: El cerebro del controlador, proporcionando capacidades de procesamiento y conectividad.
- **Conectividad USB Tipo-C**: Para una interfaz de datos y alimentación moderna y reversible.
- **Soporte NVMe**: Para almacenamiento de estado sólido de alta velocidad.
- **RP2040**: Microcontrolador secundario para tareas de tiempo real y control de periféricos.
- **Drivers de Motor**: Para el control de múltiples motores.
- **Sensores**: Integración de sensores para la percepción del entorno.
- **Compatibilidad con OAK-D-Lite**: Preparado para la integración de la cámara de visión por computadora OAK-D-Lite.

## Uso

Para abrir y trabajar con este proyecto, necesitarás KiCad 7.0 o superior. Simplemente abre el archivo `CM4_Robotics_Controller_Clean.kicad_pro` en KiCad.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, crea una rama separada para tus cambios y envía un pull request.

