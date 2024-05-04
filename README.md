<h2 align = "center"> MY MEMO FOR USING DOCKER, ALSO SCRIPT I FOUND ON INTERNET</h2>
<hr>

|          Commands                             | Behavior                            |
|---------------------------------------------  |------------------------------------ |
| `Docker ps`                                   | List processes running              |
| `docker ps -a`                                | Process status of everything        |
| `docker ps -q`                                | List IDs of all containers          |
| `docker run nginx:latest`                     | Run container in the foreground     |
| `docker run -d nginx:latest`                  | Run container in the background     |
| `docker run -d --name [name] nginx:latest`    | * Attribute name                    |
| `docker run -d -v [var/lib/docker/volume..]`  | Create and fix the container in vol | 
| `docker stop [ID_CONTAINER]`                  | Stop the container                  |
| `docker rm [ID_CONTAINER]`                    | Delete the container                |
| `docker rm -f [ID_CONTAINER]`                 | Force deletion of the container     |
| `docker rm -f $(docker ps -q)`                | Delete all active containers        |
| `docker rm -f $(docker ps -qa)`               | Delete EVERY container              |
| `docker volume create [name]`                 | Create volume                       |
| `docker volume ps`                            | List of volumes                     |
| `docker volume rm [volume_name]`              | Deletion of a volume                |
| `docker exec -it [name] bash`                 | Open container terminal             |
| `docker run -d --name c1 --mount type=bind,source=/data/,target=/usr/share/nginx/html nginx:latest` | target a bind folder and specify a source |
| `docker run -d --name c1 --mount type=bind,source=/data/,target=/usr/share/nginx/html nginx:latest` | specify a volume target
| `docker inspect`                              | List of mount                       |
| `docker inspect --format "{{.Mounts}}" [container_ID]`| Show the detail of mounting |


## Notes:

### Volumes: 
                +--------------------------------------+
                |                                      |
                |              Docker Host              |
                |                                      |
                +--------------------------------------+
                          |               |               |
                          |               |               |
          +---------------+---------+-----+------------+--------------+
          |                         |                  |               |
          |                         |                  |               |
   +------+------+      +---------+----------+      +-----+-----+    +-----+-----+
   | TMPFS     |        | Volumes:           |      | Bind      |    | Mount     |
   | (RAM disk)|        | Managed by docker  |       |      |           |    |           |
   |           |        | itself.            |
                 |      | It is independant  |
                        | of the host system.|    |           |
   +-----------+        +--------------------+      +-----------+    +-----------+
