# Identify keys

| EmployeeID | Förnamn | Efternamn | AvdelningID | E-post                       | Telefon     |
| ---------- | ------- | --------- | ----------- | ---------------------------- | ----------- |
| 201        | Erik    | Johansson | 1           | erik.johansson@coolfirma.se  | 070-1234567 |
| 202        | Anna    | Karlsson  | 2           | anna.karlsson@coolfirma.se   | 073-2345678 |
| 203        | Johan   | Andersson | 1           | johan.andersson@coolfirma.se | 072-3456789 |
| 204        | Sara    | Lindgren  | 3           | sara.lindgren@coolfirma.se   | 076-4567890 |
| 205        | Maria   | Svensson  | 2           | maria.svensson@coolfirma.se  | 070-5678901 |

a) Which columns could be candidate keys here?

b) From this set of candidate keys, which one would you choose as primary key and which ones as alternate keys?

c) Is your primary key considered as natural key or surrogate key?

d) Create another table with a primary key where one of the columns in this table could act as a foreign key.



# Solution

## a)

**Employee ID**

**E-post**

**Telefon**



## b)

**Primary Key** - **Employee ID** 

It's uniquely identifying each employee with no risk of value change.

**Alternate keys** - **E-post + Telefon**

Generally not info that you identify as Primary Key in a table even if the values are unique.

Columns often shown together with other attributes in a table with more suited Primary Key in relation to the table name.

## c)

It could be both **Natural Key** and **Surrogate Key** but more than often it is considered as a **Surrogate Key**. 

The value is generated for the system to identify the employees by numbers/ID.

In real life people identify their employees by their name and not ID.

## d)

### Salary

|SalaryID   |EmployeeID |BaseSalary|Bonus   |EffectiveDate
|-----------|-----------|----------|--------|-------------
|1          |201        |50000     |3000    |2020-04-01
|2          |202        |43000     |2500    |2020-04-01
|3          |203        |47600     |1000    |2020-04-01
|4          |204        |40000     |4000    |2020-04-01

### PK - SalaryID
Uniquely identifies ID for the salary of a certain employee.

### FK - EmployeeID
References to Employee Table