# Exercise 0_1 - Hospital task

You have this json data, convert it into three tables: Hospital, Department and Doctor. Fill these tables with data. Do this manually and not programmatically.

```json
{
  "hospital": "Sjukhusstock",
  "address": "Drottninggatan 3, Stockholm",
  "departments": [
    {
      "name": "Kardiologi",
      "doctors": [
        { "id": 1, "name": "Dr. Abra Abrahamson" },
        { "id": 2, "name": "Dr. Erika Eriksson" }
      ]
    },
    {
      "name": "Neurologi",
      "doctors": [{ "id": 3, "name": "Dr. Sven Svensson" }]
    }
  ]
}
```

### Solution

Approach
- identify entities
- identify relationships and cardinalities
- create conceptual ERD
- create tables


Initial naive conceptual ERD

<img src = "../../assets/Initial_conceptual_model.png" width=300>

**Initial tables**

Hospital

|hospital_id | name         | address          |
|------------| ----------   | -----------------|
|1           | Sjukhusstock | Drottninggatan 3|


Department

|department_id  | name         
|---------------| ----------   
| 1             | Kardiologi
| 2             | Neurologi


Doctor

|doctor_id | name         
|----------| --------
| 1        | Dr. Abra Abrahamson
| 2        | Dr. Erika Eriksson
| 3        | Dr. Sven Svensson

Refined with bridge tables to reflect many-to-many relationships

<img src = "../../assets/conceptual_exercise_hospital.png" width=500 height=250>

HospitalDepartment

|hospital_department_id | hospital_id  | department_id    |
|-----------------------| ------------ | -----------------|
| 1                     | 1            | 1                |
| 2                     | 1            | 2                |



HospitalDoctor

TODO: Left for the reader

DepartmentDoctor

TODO: Left for the reader

Test a join

Want information on Sjukhusstock and its departments
- hospital_department can join with department_id on department table and hospital_id on hospital_table
- query name from hospital table and name from department

TODO: Left for reader: create this SQL query
