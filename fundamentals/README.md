# ![[MongoDB] - Fundamentals](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to describe a MongoDB document and what its `_id` is.

## MongoDB Documents

In MongoDB, we save and retrieve *documents* to and from a *collection*.

Let's take a look at what a MongoDB *document* might look like:

```js
{
  _id: ObjectId("5099803df3f4948bd2f98391"),
  name: { first: "Alan", last: "Turing" },
  birth: ISODate("1912-06-23T00:00:00Z"),
  death: ISODate("1954-06-07T00:00:00Z"),
  contribs: [ "Turing machine", "Turing test", "Turingery" ],
  views: 1250000
}
```

As you can see, this format looks very much like a JavaScript object.

You’ll be working with documents using JavaScript; therefore, they are JS objects!

> 📚 A *collection* is a group of related *documents* within a MongoDB database. Collections serve as a container for organizing and storing documents. A *document* is a single record within a collection.

## The Document `_id`

The `_id` is a special field that represents the document’s *unique identifier*. If you’re familiar with SQL databases, a document’s `_id` is like a *primary key*.

MongoDB automatically creates the `_id` when it saves documents for the first time.

The `id` is a special `ObjectId` datatype. `ObjectId`s are JS objects, but we’ll use their *string representation* most of the time when working with them in Mongoose.

The value that MongoDB creates for the `_id` is exceptionally likely to be *globally unique*. See how MongoDB builds the value of `_id` [**here**](https://www.mongodb.com/blog/post/generating-globally-unique-identifiers-for-use-with-mongodb).