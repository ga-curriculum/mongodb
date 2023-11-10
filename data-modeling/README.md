# ![[MongoDB] - Data Modeling](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to understand what a data entity is and how different entities in a database may share relationships with each other.

## Data Entities

A **data entity** represents a specific *type* of data in an application.

Examples include **User**, **Account**, **Post**, **Comment**, **Purchase**, etc.

📚 A *data entity* is a representation of a real-world object or concept within a database. Data entities are characterized by their attributes and relationships with other data entities.

## Data Relationships

**Relationships** exist between entities, for example:

- *A User has many Purchases; a Purchase belongs to a User*
    - This relationship is called a **one-to-many**.
- *A person has visited many places; places have been visited by many people*
    - This relationship is called a **many-to-many**.

> 📚There is also a less common **one-to-one** relationship. For example, *A User has a Profile; and a Profile belongs to a User*

You are required to model the relationships as part of the planning for your CRUD projects. Here’s a [**link**](https://www.lucidchart.com/pages/er-diagrams) to **Lucidchart** that talks more about data relationships and how to create an **Entity Relationship Diagram (ERD)**.
