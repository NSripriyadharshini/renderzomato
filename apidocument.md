//Page 1
> List of city(location)
* http://localhost:9800/location

>List of restaurant
* http://localhost:9800/restaurant

>List of Restaurant wrt to City
* http://localhost:9800/restaurant?stateId=1

>List of meal type
* http://localhost:9800/mealType


//Page 2
>Restaurant wrt to meal
* http://localhost:9800/restaurant?mealId=2

>Restaurant wrt to meal & cuisine
* http://localhost:9800/filter/5?cuisineId=4

>Restaurant wrt to meal & cost
*http://localhost:9800/filter/3?hcost=500&lcost=200

>Sort on basis of cost
*http://localhost:9800/filter/3?sort=-1


//Page 3
>Details of restaurant
* http://localhost:9800/details/6

>Menu wrt to restaurant
* http://localhost:9800/menu/8


//Page 4
>Menu Details (POST)
* http://localhost:9800/menuItem
body
{
    "id":[
        3,5,7
    ]
}

>Place Order (POST)
* http://localhost:9800/placeOrder
body
{
"name": "Aakash",
"email": "aakash@gmail.com",
"address": "Hno 23,Sector 1",
"phone": 768768686,
"cost": 787,
"menuItem": [
    3,5,7
]
}


//Page 5
>List of orders
* http://localhost:9800/orders

>List of orders wrt to email
* http://localhost:9800/orders?email=anchal@gmail.com


>Update Payement Details (PUT)
* http://localhost:9800/updateOrder/65
body
{
    "status":"TXN_SUCCESS",
    "bank_name":"HDFC",
    "date":"17/11/2022"
}

>Delete Order (Delete)
* http://localhost:9800/deleteOrder/62514d8bf5aec503b2e0f2ac