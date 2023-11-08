# ![[tktk Module Name] - tktk Microlesson Name](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## Creating a Database and Inserting Documents in the Mongo Shell

Before we Start

- In this section, we will work directly with MongoDB to create and modify data using the *Mongo Shell* in a terminal window.
- However, after this first look at MongoDB, you will be better off using *Mongoose* which we will learn about next.

### The Mongo Shell

MongoDB installs with a client app, a JavaScript-based shell, to interact directly with the MongoDB engine.

Start the app in the terminal with this command:

```bash
mongo
```

The app will load, and change the prompt will change to `>`

List the shell’s commands available:

```bash
help
```

Show the list of databases:

show dbs
​
Show the name of the currently active database:
db
​
Switch to a different database:
use [name of the database to switch to]
​
Let’s switch to the local database:
use local
​
Show the collections of the current database

show collections
​
Creating a new Database

To create a new database in the Mongo Shell, we simply have to use the database. Let’s create a database named myDB:
use myDB

### Inserting Data into a Collection

This is how we can create and insert a document into a collection named *people*:

```bash
db.people.insert({
... name: "Fred",   // Don't type the dots, they are from the
... age: 21         // shell, indicating multi-line input mode
})
```

Using a collection for the first time creates it!

<aside>
🔨 **You Do: Let’s add another person to the *people* collection. But this time, add a field called *birthDate* and assign it a date value with something like this: *new Date(‘3/21/1981’)***

</aside>

To list all documents in a collection, we can use the *find* method on the collection:

```bash
db.people.find({})
```

The argument is called a *query object* and is used to specify criteria. When we provide an empty query object, `find` will return all documents.
