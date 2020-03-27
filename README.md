# Gemeente Barendrecht, Albrandswaard and Ridderkerk garbage collection in Home Assistant

Based on https://github.com/vloris/home-assistant/blob/master/custom_components/sensor/twentemilieu.py

Gemeente Barendrecht, Albrandswaard and Ridderkerk sensor for garbage collection for Home Assistant


```
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
