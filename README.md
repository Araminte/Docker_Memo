<h2 align = "center"> MY MEMO FOR USING DOCKER, ALSO SCRIPT I FOUND ON INTERNET</h2>
<hr>

|          Commands                             | Behavior                            |
|---------------------------------------------  |------------------------------------ |
| `Docker ps`                                   | List processes running              |
| `docker ps -a`                                | Process status of everything        |
| `docker ps -q`                                | List IDs of all containers          |
| `docker run nginx:latest`                     | Run container in the foreground     |
| `docker run -d nginx:latest`                  | Run container in the background     |
| `docker stop [ID_CONTAINER]`                  | Stop the container                  |
| `docker rm [ID_CONTAINER]`                    | Delete the container                |
| `docker rm -f [ID_CONTAINER]`                 | Force deletion of the container     |
| `docker rm -f $(docker ps -q)`                | Delete all active containers        |
| `docker rm -f $(docker ps -qa)`               | Delete EVERY container              |
