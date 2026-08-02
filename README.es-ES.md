

RTT
===

Código fuente de SEGGER RTT

https://www.segger.com/products/debug-probes/j-link/technology/about-real-time-transfer  
https://wiki.segger.com/RTT

## Archivos incluidos

  * `RTT/`
    * `SEGGER_RTT.c`               - Módulo principal para RTT.
    * `SEGGER_RTT.h`               - Encabezado principal para RTT.
    * `SEGGER_RTT_ASM_ARMv7M.S`    - Implementación optimizada en ensamblador de las funciones de RTT para procesadores ARMv7M.
    * `SEGGER_RTT_Printf.c`        - Implementación sencilla de printf (`SEGGER_RTT_Printf()`) para escribir cadenas con formato a través de RTT.
  * `Syscalls/`
    * `SEGGER_RTT_Syscalls_*.c`    - Llamadas al sistema de bajo nivel para redirigir `printf()` a RTT con diferentes cadenas de herramientas.
  * `Config/`
    * `SEGGER_RTT_Conf.h`          - Archivo de configuración de RTT.
  * `Examples/`
    * `Main_RTT_InputEchoApp.c`    - Aplicación de ejemplo que repite la entrada en el Canal 0.
    * `Main_RTT_MenuApp.c`         - Aplicación de ejemplo para demostrar la funcionalidad bidireccional de RTT.
    * `Main_RTT_PrintfTest.c`      - Aplicación de ejemplo para probar la implementación sencilla de printf de RTT.
    * `Main_RTT_SpeedTestApp.c`    - Aplicación de ejemplo para medir el rendimiento de RTT. (Requiere embOS)
