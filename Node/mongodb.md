# mongo Shell Methods

- db.getMongo()

      Returns the current database connection.

- show dbs

      Shows the available databases.

- use databaseName

      Uses the provided database name for the operation.

- db

      Shows the current accessing database.

- db.getName()

      Shows the current database name.

- db.createCollection(<Collection-Name>)

      Creates the provided collection name in the database.

- db.help()

      Returns the list of methods on db object.

- db.stats()

      returns a document with statistics reflecting the database system’s state.

- db.version()

      Returns the version of the mongod or mongos instance.

- db.hostInfo()

      Returns a document with information about the underlying system that the mongod or mongos runs on.

- db.dropDatabase()

      Removes the current database, deleting the associated data files.

- db.collection.count(query, options)

      Returns the count of documents that would match a find() query for the collection or view.

- db.collection.dataSize()

      Returns the size in bytes of the collection.

- db.collection.find()

      Returns the all the documents present in collection.

- db.collection.find({query})

      Returns the all the documents that matches the query from the collection.
      Example:
             db.users.find({name:"Mark"})

- db.findOne(query)

      Returns one document that satisfies the specified query criteria on the collection or view.

- db.collection.findAndModify(document)

      Modifies and returns a single document

- db.collection.insert()

      Inserts a document or documents into a collection.

- db.collection.insertOne()

      Inserts a document into a collection.

- db.collection.insertMany()

      Inserts multiple documents into a collection.

- db.collection.remove()

      Removes documents from a collection.
