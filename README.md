# Battery Regulator Module

Custom lithium-polymer battery voltage monitor and regulator module.

## Overview

This custom module is designed as a drop-in for small-scale electronics projects providing 3.3V linear regulated voltage output from a raw lithium polymer cell input. The battery input voltage is monitored by the [MIC2779](https://www.digikey.com/en/products/detail/microchip-technology/MIC2779L-2YM5-TR/1616864) whose output enables or disables the regulated output supply. It is configured with hysteresis to cutoff output when the battery voltage reaches 3.1V and to then hold in reset until the battery voltage exceeds 3.6V.

![Battery Regulator Module 3d Render](images/battery-reg-module-3d-ap7362.png)

The module supports the 1.5A maximum current limitations of the regulator chip [AP7362](https://www.digikey.com/en/products/detail/diodes-incorporated/AP7362-33SP-13/5305857) used.

This module may be combined with a Lipo charger module such as the [TP4056](https://www.best-microcontroller-projects.com/tp4056.html) (along with any in-circuit charging mods as required) for a complete custom battery charging/monitoring/regulation for small-scale electronics projects.

The zipped gerber files provided may be uploaded to a PCB manufacturer for fabrication. Below is the automatic rendering of the uploaded gerbers by [OSHPark](https://oshpark.com/home).

![Battery Regulator Module Gerbers Rendered](images/battery-reg-module-gerbers-rendered.png)

## Schematic

The schematic for the circuit is provided below as designed in Kicad 9.

![Battery Regulator Module Schematic](images/battery-reg-module-schematic.png)

## License

MIT © 2024 John Greenwell