MongoDB Contact List 
Overview

This project demonstrates basic MongoDB operations using a collection named contactlist. It includes inserting, updating, querying, and displaying contact records through the Mongo shell.

Tasks Completed

Created a new collection called contactlist.

Inserted multiple contact documents using:

db.contactlist.insertMany([...])


Displayed all documents in the collection:

db.contactlist.find().pretty()


Queried contacts with specific conditions, for example:

db.contactlist.find({ age: { $gt: 18 } })


Updated a contact’s first name from "Kefi Seif" to "Kefi Anis":

db.contactlist.updateOne(
  { last_name: "Kefi", first_name: "Seif" },
  { $set: { first_name: "Anis" } }
)

Expected Results

Documents are stored and retrieved successfully.

Queries return matching records or no results if none are found.

Updates modify only the specified fields without affecting other data.

Tools Used

MongoDB Atlas or Mongo Shell

Git Bash for command-line interaction
