---
title: "Hive SLT3B control via MQTT"
description: "Integrate your Hive SLT3B via Zigbee2MQTT with whatever smart home
 infrastructure you are using without the vendors bridge or gateway."
---

*To contribute to this page, edit the following
[file](https://github.com/Koenkk/zigbee2mqtt.io/blob/master/docs/devices/SLT3B.md)*

# Hive SLT3B

| Model | SLT3B  |
| Vendor  | Hive  |
| Description | Heating thermostat remote control |
| Exposes | battery, linkquality |
| Picture | ![Hive SLT3B](../images/devices/SLT3B.jpg) |

## Notes

### Pairing

To pair the thermostat controller to both Zigbee2MQTT and the thermostat, a factory reset will need to be performed. To begin a factory reset, press and hold both the menu and back buttons together. Allow the countdown to finish before releasing to factory reset the device. After the device has reset and a language has been selected, Zigbee2MQTT should find the device. The device should be able to control the boiler whilst still reporting to Zigbee2MQTT.

## Exposes

### Battery (numeric)
Remaining battery in %.
Value can be found in the published state on the `battery` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Linkquality (numeric)
Link quality (signal strength).
Value can be found in the published state on the `linkquality` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimal value is `0` and the maximum value is `255`.
The unit of this value is `lqi`.

