# Exercise 0_2

## Library Bookly
A library called Bookly keeps track of books and members who borrow them. Each book has a title, author, and ISBN number. Each member has a membership ID, name, and contact information. A member can borrow multiple books, but each book can be borrowed by only one member at a time.

a) Identify the entities and attributes for each entity.

b) Determine the relationship between member and books.

c) Draw a conceptual ERD using crow foots notation.

### Solution

a)
## Entities and Attributes

|Library     |Book        |Member      |
|------------|------------|------------|
|books       |title       |ID          |
|members     |author      |name        |
|            |ISBN number |contact info|


b)

Library to Book = contains

Book to Member = borrows



c)

<img src = "../assets/conceptual_exercise_2.png" width=300>