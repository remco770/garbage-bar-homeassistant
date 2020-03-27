# Garbage collection sensor for BAR for Home Assistant

Garbage collection for the following cities in the Netherlands

- Albrandswaard
- Barendrecht
- Ridderkerk

in your configuration.yaml you'll need:

```yaml
sensor:
  - platform: bar-afvalbeheer
    postcode: 0000XB
    housenumber: 1
    resources:
      - today
      - tomorrow
      - grey
      - green
      - paper
      - packages
```

It will create sensors for the next few future calendar events, called:

* sensor.bar_afvalbeheer_groente_fruit_en_tuinafval
* sensor.bar_afvalbeheer_papier_en_karton
* sensor.bar_afvalbeheer_restafval
* sensor.bar_afvalbeheer_pmd

and extra sensors:
* sensor.bar_afvalbeheer_vandaag
* sensor.bar_afvalbeheer_morgen
