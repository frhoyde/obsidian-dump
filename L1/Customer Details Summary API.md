## *Host*

[[Silicon Parser]]

## *Endpoint*

`/customer/detailsSummary`

## *Request Type*

```Json
Params: {
	username: "8801711092515"
}
```

## *Response Type*

```Json
{
    "statusCode": 1,
    "message": "suceess",
    "txId": "20250520-115121-3dbe4063",
    "data": {
		"customerDetails": {
			"id": 1,		
			"fullname": "Zakaria Ahammed",		
			"phoneNumber": "8801711092528",
			"userType": "b2c",		
			"userEmail": "zakaria.ahammed@grameenphone.com",		
			"lastLoginTime": null,	
			"invalidLoginAttempts": 0
		},
		"customerOrderTypeAndCount": {
			"totalOrders": 8196,
			"totalDevices": 8196,
			"simBasedDevices": 4867,
			"wifiBasedDevices": 2048,
			"solutions": 0
		},
		"userLastRecharge": {
			"billingType": "Prepaid",
			"lastRecharge": "2025-04-17T12:28:28"
		}
	}
}
```

## *Breakdown*


