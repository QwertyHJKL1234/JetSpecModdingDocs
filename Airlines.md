# Creating a custom airline:

Place a JSON file in the folder JetSpec_Data/Mods/Airlines

### Description:

Adds a custom airline to the game.

### Parameters:

| Parameter  | Description                        |
| ---------- | ---------------------------------- |
| name       | The name of the airline.           |
| totalMoney | The starting money of the airline. |
| prefs      | See below.                         |

### Prefs:

| Parameter     | Description                                                                            |
| ------------- | -------------------------------------------------------------------------------------- |
| efficencyPref | The preferance of the airline for buying aircraft, all three fields should add to 3.0. |
| seatsPref     | The preferance of the airline for buying aircraft, all three fields should add to 3.0. |
| rangePref     | The preferance of the airline for buying aircraft, all three fields should add to 3.0. |

### Parameters (technical):

| Parameter  | Type, Reccomended Value |
| ---------- | ----------------------- |
| name       | string, "N/A"           |
| totalMoney | long, 1000000           |
| prefs      | See below.              |

### Prefs (technical):

| Parameter     | Type, Reccomended Value |
| ------------- | ----------------------- |
| efficencyPref | float, 1.0              |
| seatsPref     | float, 1.0              |
| rangePref     | float, 1.0              |

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
}
```


