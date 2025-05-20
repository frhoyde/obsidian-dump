## *Host*

[[Silicon Parser]]

## *Endpoint*

`/customer/summary`

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
	"txId": "20250520-101850-67881091",
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
		"customerOrderStatus": {
			"newOrders": 4609,
			"firstContact": 256,
			"scheduled": 259,
			"onboarded": 1792,
			"inProgress": 1280,
			"completed": 0,
			"cancelled": 0,
			"packActivation": 256,
			"simActivation": 256
		},
		"userLastRecharge": {
			"billingType": "Prepaid",
			"lastRecharge": "2025-04-17T12:28:28"
		}
	}
}
```

## *Breakdown*

Customer Details Summary API - Customer Details, CustomerOrderTypeAndCount, BillingType ("Prepaid" if user_type == "b2c" else "Postpaid")

[[Devices And Solutions Summary API]] - CustomerOrderTypeAndCount

[[Installation Summary API]]- CustomerOrderStatus
