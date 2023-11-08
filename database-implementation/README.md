# ![[tktk Module Name] - tktk Microlesson Name](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

# Database Implementation

## SQL Databases

In SQL Databases, by design, there would be a **table** for each *data entity*.

Related data is *joined* together using SQL queries.

## MongoDB

In MongoDB, unlike with SQL tables, there might not be a **collection** for every *data entity*.

Unlike in SQL, there’s no requirement to break different *entity types* into separate **collections**.

The reason is that some *entities* are better off being **embedded** within their parent document instead, for example, *comments* that belong to a *post*. It would not make sense to query a separate **comments** collection to obtain the comments for a given post.
