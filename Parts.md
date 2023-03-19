# Creating a custom part:

Place a JSON file in the folder JetSpec_Data/Mods/Parts

### Description:

Adds a custom part to the game.

### Parameters:

| Parameter                   | Description                                                                                                  |
| --------------------------- | ------------------------------------------------------------------------------------------------------------ |
| name                        | The name of the part.                                                                                        |
| description                 | The discription of the part.                                                                                 |
| type                        | See below.                                                                                                   |
| pathToOBJ                   | The location of the .obj file, starting at JetSpec\_Data.                                                    |
| efficiency                  | Only applies to engines: Efficiency of the engine (from 0-1)                                                 |
| cruisingSpeedMach           | Only applies to engines: Cruising speed of the engine in mach                                                |
| takeoffThrust               | Only applies to engines: Takeoff thrust in kN                                                                |
| weight                      | Only applies to engines: Weight of the engine                                                                |
| twr                         | Only applies to engines: Thrust-to-weight ratio                                                              |
| cost                        | Only applies to engines: Cost of the engine                                                                  |
| costPerSqrMeter             | Applies to all but engine: Cost per sqr meter                                                                |
| buildMaterial               | Applies to all but engine: See below                                                                         |
| weightPerSqrMeter           | Applies to all but engine: WeightPerSqrMeter, in KG                                                          |
| isFBW                       | Only applies to cockpits: Is it fly-by-wire?                                                                 |
| containsFuel                | Only applies to wings: Does it contain fuel tanks?                                                           |
| hasWinglets                 | Only applies to wings: Does it have winglets?                                                                |
| wingletType                 | Only applies to wings: See below.                                                                            |
| numberofVerticalStabilizers | Only applies to Vertical Stabilizers: How many tails does it have?                                           |
| onEndOfHorizontalStabilizer | Only applies to Vertical Stabilizers: Are the vertical stabilizers on the end of the horizontal stabilizers? |
| mountType                   | Only applies to Horizontal Stabilizers: See below.                                                           |

### Prefs:

| Parameter     | Description                                                                                                      |
| ------------- | ---------------------------------------------------------------------------------------------------------------- |
| efficencyPref | The preferance of the airline for buying aircraft, all three fields should add to 3.0. (Unless using skipChecks) |
| seatsPref     | The preferance of the airline for buying aircraft, all three fields should add to 3.0. (Unless using skipChecks) |
| rangePref     | The preferance of the airline for buying aircraft, all three fields should add to 3.0. (Unless using skipChecks) |

### Parameters (technical):

| Parameter  | Type, Reccomended Value |
| ---------- | ----------------------- |
| name       | string, "N/A"           |
| totalMoney | long, 1000000           |
| prefs      | See below.              |
| skipChecks | bool, false             |

### Prefs (technical):

| Parameter     | Type, Reccomended Value |
| ------------- | ----------------------- |
| efficencyPref | float, 1.0              |
| seatsPref     | float, 1.0              |
| rangePref     | float, 1.0              |

## IMPORTANT: MAKE SURE PREFS ALL ADD TO 3.0 (Unless using skipChecks)

### Example:

```json
{
  "name": "AirAccess",
  "totalMoney": 12000000000,
  "prefs": {
    "efficencyPref": 1.0,
    "seatsPref": 0.5,
    "rangePref": 1.5
  },
  "description": "AirAccess is a long haul carrier flying to and from their hub in Athens, Greece. They prioritize being able to fly to almost everywhere on the globe."
  "skipChecks": false
}
```
