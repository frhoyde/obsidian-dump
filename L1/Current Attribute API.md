## *Host*

[[Silicon Parser]]

## *Endpoint*

`/attributes/currentAttributes`

## *Request Type*

```Json
{
	"txId":"abcd",
	"imeiList": ["867232055980248", "867232055968466", "867232055731245"]
}
```

## *Response Type*

```Json
{
    "statusCode": 1,
    "message": "success",
    "txId": "abcd",
    "data": {
        "currentAttributes": [
            {
                "imei": "867232055731245",
                "latitude": 22.685981666666667,
                "longitude": 90.64595783333333,
                "locationTime": "2025-05-15 17:32:38",
                "speed": 0.0,
                "ignition": false,
                "motion": false,
                "batteryLevel": null,
                "obdOdometer": null,
                "tripFuel": null,
                "tripOdometer": null,
                "fuel": null,
                "fuelConsumption": null,
                "rpm": null,
                "engineLoad": null,
                "power": null,
                "eventStatus": "deviceOffline",
                "lastEvent": "deviceOffline",
                "lastEventTime": "2025-05-15 18:16:58",
                "coolantTemp": null,
                "airTemp": null,
                "intakePressure": null,
                "throttle": null,
                "fuelUsed": null,
                "course": 264.0,
                "satellite": null,
                "validity": true,
                "gsmSignal": null,
                "altitude": 0.0,
                "totalDistance": 383454.0,
                "address": "Bhola, Bhola Sadar Subdistrict, Bhola District, Barishal Division, Bangladesh",
                "sensorTemperature": null,
                "poiDetails": null
            },
        ]
    }
}
```

## *Breakdown*

| Field            | Type     | Description                                           |
|------------------|----------|-------------------------------------------------------|
| imei             | String   | Vehicle/Device Unique ID                              |
| latitude         | Float    | Location latitude                                     |
| longitude        | Float    | Location longitude                                    |
| locationTime     | String   | Time of location retrieval (Format: `YYYY-MM-DD HH:mm:ss`) |
| speed            | Float    | Vehicle speed                                         |
| ignition         | Boolean  | If the engine is on                                   |
| motion           | Boolean  | If the vehicle is in motion                           |
| batteryLevel     | Float    | Battery level                                         |
| obdOdometer      | Int      | Odometer information                                  |
| tripFuel         | Float    | Trip fuel consumption                                 |
| tripOdometer     | Long     | Trip total distance                                   |
| fuel             | Float    | Fuel level                                            |
| fuelConsumption  | Float    | Fuel consumption rate                                 |
| rpm              | Float    | Engine RPM                                            |
| engineLoad       | Null     | Engine load                                           |
| power            | Null     | Power output                                          |
| eventStatus      | String   | Event status (e.g., "deviceOffline")                  |
| lastEvent        | String   | Last event (e.g., "deviceOffline")                    |
| lastEventTime    | String   | Last event timestamp                                  |
| coolantTemp      | Null     | Coolant temperature                                   |
| airTemp          | Null     | Air temperature                                       |
| intakePressure   | Null     | Intake pressure                                       |
| throttle         | Null     | Throttle position                                     |
| fuelUsed         | Null     | Total fuel used                                       |
| course           | Float    | GPS course heading                                    |
| satellite        | Null     | Satellite data                                        |
| validity         | Boolean  | If the location data is valid                         |
| gsmSignal        | String   | Signal strength                                       |
| altitude         | Float    | Altitude                                              |
| totalDistance    | Float    | Total distance traveled                               |
| address          | String   | Human-readable location                               |
| sensorTemperature| Null     | Sensor temperature                                    |
| poiDetails       | Null     | Point of interest details                             |

## Tags

#API
