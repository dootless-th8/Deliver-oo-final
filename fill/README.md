# oo_delivery.py

## Ovrview
This project is about creating delivery service that utilise oop programming formula

## Feature
* ### class Person:
       Can say Hi
    #### Customer (Inherit):
        Can order things
        !!composit of DeliveryOrder
    #### Driver (Inherit):
        Delivers order
        !!composit of DeliveryOrder
* ### class Person:
        has order info
        can change detemine status of the order

## How to run
Create driver and customer objects first, then assigned the order of each customers. 
Enjoy

Examples:
```bash
alic = Customer("Alice", "Idaho")
print(alic.introduce())

bb = Customer("Bob", "Bannna")
print(bb.introduce())

dvd = Driver("David", "motorcycle")
print(dvd.introduce())

print()
# summ
or1 = alic.place_order("Laptop")
or1.assign_driver(dvd)
or2 = bb.place_order("Headphones")
or2.assign_driver(dvd)


print(or1.summary())
print(or2.summary())

dvd.deliver(or1)
dvd.deliver(or2)

print()

print(or1.summary())
print(or2.summary())

```

## Project Structure
```bash
|-fill
|   --oo_delivery.py    # The program
|   --README.md         #This file
|   --res.png           #Evidence
```