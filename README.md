# KiCad Projects

Schematics, PCB layouts and component libraries I designed in **[KiCad](https://www.kicad.org/)** during my first year of Computer Engineering at KNUST.

## Projects

| Project | Description | Key components |
|---|---|---|
| [`gas-detector-system`](projects/gas-detector-system) | **IoT gas detection system built under a mentorship programme.** The ESP32-C3 reads the gas sensors, sounds a buzzer alarm, and publishes readings over **MQTT** to a custom web dashboard for remote monitoring. Includes the schematic, a power unit sheet and the **PCB layout**. | ESP32-C3 SuperMini, gas sensors, buzzer, MQTT |
| [`project-c-10`](projects/project-c-10) | Climate-controlled relay switch: reads temperature and humidity and switches a load | ESP32-C3-DevKitM-1, DHT22, relay |
| [`food`](projects/food) | Fan control circuit for a food preservation/drying unit, driven through a transistor-switched relay | ESP32-C3-DevKitM-1, S8050 BJT, relay, 1N4007, fan |
| [`lab1-sensor-report`](projects/lab1-sensor-report) | EE lab 1: multi-sensor circuit, with diagram and code screenshots for the report | ESP32-C3, DHT11, HC-SR04, LM2903 comparator |
| [`codefest-2026`](projects/codefest-2026) | Codefest 2026 hackathon circuit: push buttons, potentiometer input and LED output | Arduino UNO R3, potentiometer, switches, LED |

## Component libraries

Custom symbols, footprints and 3D models (`.step`) used by the projects:

| Library | Part |
|---|---|
| [`ESP32-C3_SUPERMINI_TH`](libraries/ESP32-C3_SUPERMINI_TH) | ESP32-C3 SuperMini module (through-hole) |
| [`DHT22`](libraries/DHT22) | DHT22 temperature & humidity sensor |
| [`HC-SR04`](libraries/HC-SR04) | HC-SR04 ultrasonic distance sensor |
| [`LM393`](libraries/LM393) | LM393 dual comparator (SO-8) |

## Opening a project

1. Install **KiCad 8** or later.
2. Open the `.kicad_pro` file inside a project folder.
3. If a symbol shows as missing (`?`), add the matching library:
   **Preferences → Manage Symbol Libraries → Project Specific Libraries → ➕** and pick the `.kicad_sym` file from `libraries/`.
   Do the same for footprints under **Manage Footprint Libraries**, using the `.kicad_mod` folder.
   Each library also has a `how-to-import.htm` guide.

## Related

- [voltguard-pcb](https://github.com/Oscar006-HUB/voltguard-pcb): VoltGuard board built on the ESP32-C3 SuperMini
- [proteus-projects](https://github.com/Oscar006-HUB/proteus-projects): circuit simulations in Proteus

---

Author: **Prince Oscar Mwinnuo** ([@Oscar006-HUB](https://github.com/Oscar006-HUB))
