Run a mongo container:
docker compose up

Execute this command to access the container:
docker exec -it \<container_id\> bash

Inside container try this to connect on mongo:
mongosh -u admin -p admin
![image](https://github.com/user-attachments/assets/c6eb8290-5b47-462b-9cb3-3133ceca27c8)

Commands using shell:
list databases:
show dbs

Display essentials commands in mongo:
db.help()

mongodb statistics:
db.stats()

Create database/select database:
use \<database_name\>

Insert document in database:
db.\<database_name\>.insert({"id":"21334"})
example: db.user.insertOne({"document":"123456","name": "John","age":35})

to get all objects:
db.<db_name>.find()

Droping database:

use \<database_name\>
db.dropDatabase()

filter documents by specific field:<br/>
 db.user.find({document:'122334343'})

 
Commands using MongoDB Query Language (MQL):

Filter all documents:
- Filter all collection documents: \{\}
- Filter documents that contains "status" field equals "D": \{ status: "D" \}
- Filter documents that document field is equals '32678456385' or '32678443285': <br/>
    {$or:[ {document: '32678456385'},{ document: '32678443285'}]}
