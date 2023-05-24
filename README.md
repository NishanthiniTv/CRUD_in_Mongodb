# CRUD_in_Mongodb
To perform CRUD operations using MongoDB
#Prerequisites
Before running the application, ensure that you have the following:

MongoDB installed and running.
A MongoDB database and collection set up for storing book records.
A server environment capable of running the HTML code (e.g., Node.js with Express.js).
Install the dependencies: 'npm i --s express express-handler body-parser mongodb express-handlebars' and 'npm i -g nodemon'

#MongoDB CRUD Operations:
The HTML code interacts with MongoDB through the following routes/endpoints:

/store_values: Handles the creation of a new book record. It receives the data from the "Create" form and inserts a new document into the MongoDB collection.

/update_values/{{edit_id}}: Updates an existing book record. It receives the updated data from the "Edit" form and modifies the corresponding document in the MongoDB collection based on the edit_id parameter.

/?edit_id={{this._id}}: Triggers the display of the "Edit" section with pre-filled form fields for the selected book record. The edit_id query parameter identifies the specific book to be edited.

/?delete_id={{this._id}}: Initiates the deletion of a book record. It prompts for confirmation and, if accepted, removes the corresponding document from the MongoDB collection. The delete_id query parameter specifies the book to be deleted.
