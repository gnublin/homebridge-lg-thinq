## Washer / WashTower / Dryer

```json
{
    "id": "911fad63-****-****-****-*******",
    "name": "Washer",
    "washer_trigger": true,
    "washer_door_lock": true
}
```

* `id` required, device id
* `name` optional, device display name
* `washer_trigger` default `false`, enable program finished trigger? worked as Occupancy sensor
* `washer_door_lock` default `false, enable door lock status

## Air Conditioner

```json
{
    "id": "911fad63-****-****-****-*******",
    "name": "AC",
    "ac_air_quality": true,
    "ac_mode": "BOTH",
    "ac_swing_mode": "VERTICAL",
    "ac_temperature_sensor": false,
    "ac_fan_control": false,
    "ac_buttons": [
        {
            "name": "Cool",
            "op_mode": 0
        },
        {
            "name": "Energy Saver",
            "op_mode": 6
        },
        {
            "name": "Fan",
            "op_mode": 2
        },        {
            "name": "Heat",
            "op_mode": 4
        },
        {
            "name": "Dry",
            "op_mode": 1
        }
    ],
}
```

* `id` required, device id
* `name` optional, device display name
* `ac_air_quality` default `false`, enable air quality sensor (if your device supported)
* `ac_mode` default `BOTH`, your AC mode, select `COOLING` for cooling mode, `HEATING` for heating mode or `BOTH` if your AC supported both of cooling and heating
* `ac_swing_mode` default `BOTH`, your AC swing mode, `VERTICAL` swing mode, `HORIZONTAL` swing mode or `BOTH`, this mode will turn on/off swing mode only, cannot control specified swing direction
* `ac_temperature_sensor` default `false`, enable current temperature as sensor if you want setup automation
* `ac_led_control` default `false`, enable led panel control (if your device supported)

## Refrigerator

```json
{
    "id": "911fad63-****-****-****-*******",
    "name": "Refrigerator",
    "ref_express_freezer": true,
    "ref_express_fridge": true,
    "ref_eco_friendly": false
}
```

* `id` required, device id
* `name` optional, device display name
* `ref_express_freezer` default `false`, enable Freezer / Ice Plus switch
* `ref_express_fridge` default `false`, enable Express Fridge switch
* `ref_eco_friendly` default `false`, enable Eco Friendly switch