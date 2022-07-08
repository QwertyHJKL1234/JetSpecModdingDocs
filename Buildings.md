# Creating a custom building:



### Description:

Adds a custom building to the game.



### Parameters:

| name            | The name of the building                                                                                                     |
|:---------------:|:----------------------------------------------------------------------------------------------------------------------------:|
| cost            | The cost to place the building                                                                                               |
| textureLocation | The location of the texture, starting at JetSpec\_Data                                                                       |
| buff            | DEPRECATED, SET TO "null"                                                                                                    |
| description     | The description of what the building does                                                                                    |
| type            | An enum, can be set to "util", "office", "design", "factory", "hq", "runway", "hanger", or "demolish"                        |
| level           | The level of the building, set from 1-5.                                                                                     |
| scale           | The scale of the image in textureLocation, this is mostly trial and error to see what size you like. WIP texture uses 10x10. |

### Parameters (technical):

| **Parameter**   | **Type, Reccomended Value**                                             |
|:---------------:|:-----------------------------------------------------------------------:|
| name            | string, "N/A"                                                           |
| cost            | long, 100000                                                            |
| textureLocation | string (filepath), "Data/Textures/WIP.png"                              |
| buff            | string, "null"                                                          |
| description     | string, "N/A"                                                           |
| type            | [BuildingType](#buildingtype-enum), "util"                              |
| level           | int, 1                                                                  |
| scale           | Vector3, {"x":10.0,"y":1.0,"z":10.0,"magnitude":0.0,"sqrMagnitude":0.0} |

### Example:

```json
{
    "name":"Level 2 Factory", 
    "cost":500000000, 
    "textureLocation":"Data/Textures/Factory_lvl_2", 
    "buff":"null", 
    "description":"A place to build planes, slowly.", 
    "type":"factory", 
    "level":2, 
    "scale":{"x":15.0,"y":1.0,"z":15.0,"magnitude":0.0,"sqrMagnitude":0.0}
}
```



------

# BuildingType (enum)
