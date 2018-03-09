Yellow Pages on RESTful API using Binary Trees

The Yellow Pages allows you to store Person information in a binary tree. The approach was used to make sure retrieves, deletes and inserts are faster than normal array like data structures.

Person class stores the following information -
personID
FirstName
LastName
Organization
Address
contactNo
isCurrent
The BST is based on personID and it allows duplicates. This was to make sure that a person can have more than one address or can change his/her information in future. The isCurrent helps us to figure out if the information is the current or a history record. 
The deletions in this BST are not based on isCurrent. This was done keeping in mind that the API allows DELETES.

Instructions to run the API - 
GET - api/YelowPage - Will display all persons present in the dictionary.

GET - api/YelowPage/{id} - Will display person(s) with a personID = {id}.

GET - api/YelowPage/{id}/{history} - Will display person’s historical data.

POST - api/YelowPage - Allows you to create new entry to yellow page.

PUT - api/yelowPage/{id} - allows you to update information.

DELETE - api/yelowPage/{id} - allows you to delete information.
