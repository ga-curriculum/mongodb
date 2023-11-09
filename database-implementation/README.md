# ![[MongoDB] - Database Implementation](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## MongoDB

In MongoDB, unlike with *SQL tables*, there might not be a **collection** for every *data entity*.

Unlike in SQL, there’s no requirement to break different *entity types* into separate **collections**.

The reason is that some *entities* are better off being **embedded** within their parent document instead of being referenced from a separate **collection**. For example, *comments* that belong to a *post* would not be ***referenced*** by multiple posts, or even by another **entity** from a different **collection.** It would not make sense to query a separate **comments** collection to obtain the comments for a given post. This also increases the efficiency of an app.
