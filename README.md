# Amusement Park Management System (APMS)


---

## Introduction

The **Amusement Park Management System (APMS)** is designed to streamline operations in a theme park.  
It manages customer admissions, rides, food outlets, gift shops, employee tasks, and safety inspections, ensuring a smooth and enjoyable experience for visitors while maintaining operational efficiency. This system ensures **efficient park management** while improving the overall experience for visitors and staff alike.

---

## Key Features

- Manage customer admissions and ticketing  
- Track vehicle parking and ride usage  
- Organize zones and rides within the park  
- Handle food outlets, menus, and customer food purchases  
- Manage gift shops and merchandise sales  
- Record maintenance and safety inspections for rides  
- Organize employees and departments  

---

## Entities

- **Customer** - Park visitors  
- **Ticket** - Admission passes  
- **Parking** - Vehicle parking slots  
- **Zone** - Themed park areas  
- **Ride** - Park attractions  
- **SafetyInspection** - Ride safety checks  
- **Department** - Staff organizational units  
- **Employee** - Park workers  
- **FoodOutlet** - Dining locations  
- **FoodItem** - Menu items  
- **GiftShop** - Retail stores  
- **Merchandise** - Shop products  
- **Maintenance** - Ride repair records  
- **CustomerRide** - Customer ride experiences  
- **BuysFood** - Food purchase records  
- **BuysMerchandise** - Merchandise purchase records  

---

## Relationships

- **Customer → Ticket (1:1)** - One customer purchases one ticket  
- **Customer → Parking (1:1)** - One customer uses one parking slot  
- **Zone → Ride (1:M)** - One zone contains multiple rides  
- **Ride → SafetyInspection (1:M)** - One ride requires multiple safety inspections  
- **Department → Employee (1:M)** - One department employs multiple employees  
- **Customer ↔ Ride (M:M)** - Many customers can ride many rides (via CustomerRide)  
- **Zone → FoodOutlet (1:M)** - One zone has multiple food outlets  
- **FoodOutlet → FoodItem (1:M)** - One outlet offers multiple food items  
- **Customer ↔ FoodItem (M:M)** - Customers buy multiple food items (via BuysFood)  
- **Zone → GiftShop (1:M)** - One zone has multiple gift shops  
- **GiftShop → Merchandise (1:M)** - One shop stocks multiple merchandise items  
- **Customer ↔ Merchandise (M:M)** - Customers buy multiple merchandise (via BuysMerchandise)  
- **Ride → Maintenance (1:M)** - One ride needs multiple maintenance records  
- **Employee → Maintenance (1:M)** - One employee performs multiple maintenance tasks  
- **Employee → SafetyInspection (1:M)** - One employee conducts multiple safety inspections  

---
**Author:** Sai Surya Pranav Biraka

