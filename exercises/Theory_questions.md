# Theoretical questions

## a) What is a conceptual data model, and why is it important?

It is a high-level representation of data using relations (tables), usually created using ERD. 

    - It gives stakeholders a clear understanding of data.

    - Relationships and business rules will be captured before implementation.
    
    - Guides the design for the logical and physical database.

## b) Storing age in a database, is that a good idea, why?

It is not good since age changes with time.
Better to store a certain start date/date of birth and calculate it dynamically when you want the age in a certain scenario.

## c) What are the three types of data structures, and how do they differ?



## d) Give examples of how each data structure is used in real-world applications

## e) What is cardinality in data modeling, and why is it important?

It defines the relationship between tables.

    - Helps structure the relationships (one-to-one, one-to-many, many-to-many)

    - Impacts performance and integrity in the database.

## f) What are the different steps of data modeling?

    - Conceptual model
        Defines entities, attributes and relationships

    - Logical model
        Translates the conceptual model into a structured schema.

    - Physical model
        Implements the logical model in a database management system.

## g) What factors influence the choice between using an RDBMS and NoSQL?