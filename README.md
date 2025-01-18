Run a mongo container:
docker compose up

Execute this command to access the container:
docker exec -it \<container_id\> bash

Inside container try this to connect on mongo:
mongosh -u admin -p admin
![image](https://github.com/user-attachments/assets/c6eb8290-5b47-462b-9cb3-3133ceca27c8)


