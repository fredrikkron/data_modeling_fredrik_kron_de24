# Conceptual ERD to words

This is an ERD conceptual diagram that a database designer and the business stakeholders agreed upon in a car rental company called Carent.

<img src = "../assets/image.png" width=300>

a) Describe the entities in this conceptual ERD.

b) Write out the relationship labels.

c) Describe the relationships between the entities (one-to-many, one-to-one and many-to-many).

d) Define the relationship statement for example: "A Customer can have one or more Rentals".

## Solution

a)

***Customer - The individuals that rent cars from the company.***

***Rental - The transaction between Customer and Car.***

***Car - The vehicles that are avaiable for rent.***

b)

Customer ***Makes*** Rental

Rental ***Assigned to*** Car

<img src = "../../assets/image_2_b.png" width=500>


c)

***Customer --> Rental*** = one-to-many

***Car --> Rental*** = one-to-many

***Customer --> Car*** = many-to-many

d)

### Customer --> Rental

Each ***Customer*** can do more than one ***Rental***, but each ***Rental*** is connected to only one ***Customer***.

### Car --> Rental

Each ***Car*** can be rented one or more times, but each ***Rental*** only has one car at a time


### Customer --> Car

A ***Customer*** can rent multiple cars and a ***Car*** can be rented by multiple customers.
