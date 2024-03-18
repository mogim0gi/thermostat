# thermostat
home assistant thermostat config: goes into configuration.yaml


climate svetaine_termostatas:
  - platform: generic_thermostat
    unique_id: thermo4
    name: "Svetaine Termostat"
    heater: switch.1a_kolektorius3
    target_sensor: sensor.svetaine_ir_virtuve
    min_temp: 15
    max_temp: 25
    ac_mode: false
    cold_tolerance: 0.1
    hot_tolerance: 0
    keep_alive:
      minutes: 1
    precision: 0.5
    away_temp: 15
