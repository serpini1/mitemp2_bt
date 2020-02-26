# Mitemp2_bt

Support for Xiaomi Mi Temp 2 BLE environmental sensor based in [HA mitemp_bt component](https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/mitemp_bt/) and [mitemp library](https://github.com/ratcashdev/mitemp) of [@ratcashdev](https://github.com/ratcashdev).

## Installation

For install have three ways:

* Download this repository and extract to <config directory>/custom_components/mitemp2_bt
* Add custom repository to HACS (Home Assistant Community Store).
* By HACS (Home Assistant Community Store) -> COMING SOON.

## Configurartion

The config it's the samme of [mitemp_bt component](https://www.home-assistant.io/integrations/mitemp_bt/) execpt the platform field, for example:
  <br><br>

```yaml
sensor:
    - platform: mitemp2_bt
    mac: 'xx:xx:xx:xx:xx:xx'
    name: example
    force_update: true
    timeout: 60
    median: 1
    monitored_conditions:
        - temperature
        - humidity
        - battery
```