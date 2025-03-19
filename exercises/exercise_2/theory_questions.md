# Theoretical questions
a) What are the differences between first, second, third normal forms?

b) Can a normalized design still have flaws? Can you come up with example where this might happen?

c) If a > b and b > c, then a > c. What could this pattern be called?

d) When is ternary relationship needed?

e) In general how far do you need to normalize your design?

f) What's the purpose of normalizations?

g) Is a ternary relationship a bridge table

# Answer

a) 

**first normal form**
- row order doesn't matter
- Primary Key in each table
- no repeating groups
- uniform column data

**second normal form**
- 1NF
- non prime attributes, must be functionally dependent on entire pk and not just part of it

**third normal form**
- 2NF
- non prime attributes depends on the key, the whole key and nothing but the key

b) 

Complexity, performance issues and loss of meaning/understanding can appear.

If you have too many tables, it can be harder to make database maintenance.

Excessive normalization increases the amount of joins to do which can slow queries.

Over-normalization can make it harder to understand connections and remove useful redundancy.

**Example:** 

You have a patient history at a hospital across multiple normalized tables.

Making queries to retrieve the full medical history of that patient may require multiple complex joins in different tables which can degrade performance.

That is why in some cases it is better to denormalize for a more efficient database.

c)

It could be called a transitive dependancy that is adressed in 3NF when talking about databases.

That is a functional dependancy where one non-key attribute is dependent on another non-key attribute in a database table which isn't okay in 3NF.

d)

When three entities have a direct meaningful relationship that cannot be decomposed into simpler relationships without losing important information.

**Employee**, **Project**, **Role**

The Role is only meaningful in context of both an Employee and a Project so a ternary relationship is useful here.

e)

3NF is often reasonably enough.

In that form the redundancy is minimized to prevent anomalies and the performance is optimized.

f)

The purpose is to:

- Reduce redundancy
- Ensure data integrity and consistency
- Prevent anomalies (insert, update and delete)
- Make maintenance easier

g)

A ternary relationship is often implemented as a bridge table with foreign keys referencing the three related entities.

Ternary relationship models a three entity real-world scenario.

A bridge table is used to resolve many-to-many relationships.