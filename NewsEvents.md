# Creating a custom news event:

Place a JSON file in the folder JetSpec_Data/Mods/NewsEvents.

### Description:

Adds a custom news event to the game.

### Parameters:

| Parameter       | Description                                                            |
| --------------- | ---------------------------------------------------------------------- |
| name            | The name of the event, only referenced in code.                        |
| headline        | Headline of the news article, all in caps.                             |
| eventText       | The body text of the news article.                                     |
| dateTimeOfEvent | The date of the event. MUST HAVE THE TIME BE 00:00:00                  |
| buff            | The effect of the event.                                               |
| buffLengthDays  | The length of the buff, in days.                                       |
| oilPriceChange  | If you want oil price to change after the event. (NOT IMPLEMENTED YET) |
| partNameChange  | Which part should be affected by the price change below.               |
| partPriceChange | The change of price of the part named above.                           |

### Parameters (technical):

| Parameter       | Type, Reccomended value       |
| --------------- | ----------------------------- |
| name            | string, "N/A"                 |
| headline        | string, "N/A"                 |
| eventText       | string, "N/A"                 |
| dateTimeOfEvent | DateTime, 1964-12-08T00:00:00 |
| buff            | float, 1.0                    |
| buffLengthDays  | int, 10                       |
| oilPriceChange  | float, 1.0                    |
| partNameChange  | string, "Part"                |
| partPriceChange | float, 1.0                    |

### Example:

```json
{
  "name": "IADOpening",
  "headline": "NEW D.C. AIRPORT",
  "eventText": "Dulles International Airport opened today, and it is the first airport designed to handle jet aircraft.",
  "dateTimeOfEvent": "1962-11-17T00:00:00",
  "buff": 1.5,
  "buffLengthDays": 25,
  "oilPriceChange": 1.0,
  "partNameChange": "Part",
  "partPriceChange": 1.0
}

```
