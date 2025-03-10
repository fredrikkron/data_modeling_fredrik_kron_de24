# Exercise 0_2

## Library Bookly
A library called Bookly keeps track of books and members who borrow them. Each book has a title, author, and ISBN number. Each member has a membership ID, name, and contact information. A member can borrow multiple books, but each book can be borrowed by only one member at a time.

a) Identify the entities and attributes for each entity.

b) Determine the relationship between member and books.

c) Draw a conceptual ERD using crow foots notation.

### Solution

a)
## Entities and Attributes

|Library     |Book        |Member      |Borrowing   |
|------------|------------|------------|-------------
|library_id  |book_id     |member_id   |borrow_id   |
|name        |title       |name        |book_id     |
|location    |author      |contact_info|member_id   |
|            |library_id  |            |borrow_date |
|            |isbn        |            |return_date |

b)

borrowing

c)

<img src = "../assets/0_2_b.png" width=300>