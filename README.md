<h2 align = "center"> MY MEMO FOR USING DOCKER, ALSO SCRIPT I FOUND ON INTERNET</h2>
<hr>

## LISTING OF CONTAINERS

| Command                           | Explanations                                                      |
|:---------------------------------:|:------------------------------------------------------------------|
| Docker ps                         | List process who's running (ps = process status)                  |
| docker ps -a                      | Process status of everything                                      |
| docker ps -q                      | List IDs of all containers                                        | 

---
|| ## CREATION OF CONTAINERS                                                                            |

| Command                           | Explanations                                                      |
|:---------------------------------:|:------------------------------------------------------------------|
| docker run nginx:latest           | Running container in the foreground, it occupies the terminal     |
| docker run -d nginx:latest        | Running container in the background and allow us to continue      |

---
## MANAGEMENT OF CONTAINERS 

| Command                           | Explanations                                                      |
|:---------------------------------:|:------------------------------------------------------------------|
| docker stop [ID_CONTAINER]        | Stop the container                                                |
| docker rm [ID_CONTAINER]          | Delete the container                                              |
| docker rm -f [ID_CONTAINER]       | Force the deletion of the container                               |
| docker rm -f $(docker ps -q)      | Delete every active containers                                    |
| docker rm -f $(docker ps -qa)     | Delete EVERY containers                                           |            

## LISTING OF CONTAINERS

| Command                  | Explanations                                                               |
|:------------------------:|:---------------------------------------------------------------------------|
| Docker ps                | List processes that are running (ps = process status)                      |
| docker ps -a             | Process status of everything                                               |
| docker ps -q             | List IDs of all containers                                                 | 

---

## CREATION OF CONTAINERS

| Command                           | Explanations                                                      |
|:---------------------------------:|:------------------------------------------------------------------|
| docker run nginx:latest           | Run container in the foreground, occupying the terminal           |
| docker run -d nginx:latest        | Run container in the background, allowing continuation            |

---

## MANAGEMENT OF CONTAINERS 

| Command                           | Explanations                                                      |
|:---------------------------------:|:------------------------------------------------------------------|
| docker stop [ID_CONTAINER]        | Stop the container                                                |
| docker rm [ID_CONTAINER]          | Delete the container                                              |
| docker rm -f [ID_CONTAINER]       | Force deletion of the container                                   |
| docker rm -f $(docker ps -q)      | Delete all active containers                                      |
| docker rm -f $(docker ps -qa)     | Delete EVERY container                                            |
