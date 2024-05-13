<h2 align = "center"> MY MEMO FOR USING DOCKER, ALSO SCRIPT I FOUND ON INTERNET</h2>
<hr>

|          Commands                             | Behavior                            |
|---------------------------------------------  |------------------------------------ |
| `Docker ps`                                   | List processes running              |
| `docker ps -a`                                | Process status of everything        |
| `docker ps -q`                                | List IDs of all containers          |
| `docker images`                               | List images                         |
| `docker network ls`                           | Analyze the type of network         |
| `docker inspect [network_ID]`                 | Inspect caract of network (gateway..)| 
| `docker run nginx:latest`                     | Run container in the foreground     |
| `docker run -d nginx:latest`                  | Run container in the background     |
| `docker run -d --name [name] nginx:latest`    | * Attribute name                    |
| `docker run -d -v [var/lib/docker/volume..]`  | Create and fix the container in vol | 
| `docker run -d debian:latest sleep infinity`  | UNIX command that pauses the process, infinite puts the process active indefinitely |
| `docker run -d debian:latest -u [user_ID]`    | Default connexion with the USER_ID  | 
| `docker stop [ID_CONTAINER]`                  | Stop the container                  |
| `docker rm [ID_CONTAINER]`                    | Delete the container                |
| `docker rm -f [ID_CONTAINER]`                 | Force deletion of the container     |
| `docker rm -f $(docker ps -q)`                | Delete all active containers        |
| `docker rm -f $(docker ps -qa)`               | Delete EVERY container              |
| `docker volume create [name]`                 | Create volume                       |
| `docker volume ps`                            | List of volumes                     |
| `docker volume rm [volume_name]`              | Deletion of a volume                |
| `docker exec -it [name] bash`                 | Open container terminal             |
| `docker ext -it [id_container] -u [user] bash`| Connexion as $userid                | 
| `docker run -d --name c1 --mount type=bind,source=/data/,target=/usr/share/nginx/html nginx:latest` | target a bind folder and specify a source |
| `docker run -d --name c1 --mount type=bind,source=/data/,target=/usr/share/nginx/html nginx:latest` | specify a volume target
| `docker inspect`                              | List of mount                       |
| `docker inspect --format "{{.Mounts}}" [container_ID]`| Show the detail of mounting |
| `docker run -d --name [ID] -p [Host_Port]:[DockerPort] nginx:latest` | Declaration of the port between the host and container [Port forwarding 8080 to host to 80 in container] |
| `docker network create --driver=bridge --subnet[ip/netmask] [network_name]` | Create network |    
| `docker network connect [ID_network] [ID_container]` | Add virtual Interface in the network ID, it keeps docker0 network |
| `docker run -d --name [container_ID] --network host yyy`| Driver host, Bypass the bridge and share the same IP as the host |  
