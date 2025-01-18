Run a mongo container:
docker compose up

Execute this command to access the container:
docker exec -it \<container_id\> bash

Inside container try this to connect on mongo:
mongosh -u admin -p admin
![image](https://github.com/user-attachments/assets/c6eb8290-5b47-462b-9cb3-3133ceca27c8)

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

Droping database:

use \<database_name\>
db.dropDatabase()

