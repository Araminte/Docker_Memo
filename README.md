<h2 align = "center"> MY MEMO FOR USING DOCKER, ALSO SCRIPT I FOUND ON INTERNET</h2>
<hr>

|          **LISTING OF CONTAINERS**          |                                     |
|---------------------------------------------|------------------------------------ |
| **Command**                                 | **Explanations**                    |
| Docker ps                                   | List processes running              |
| docker ps -a                                | Process status of everything        |
| docker ps -q                                | List IDs of all containers          |
|                                             |                                     |
|         **CREATION OF CONTAINERS**          |                                     |
|                                             |                                     |
| docker run nginx:latest                     | Run container in the foreground     |
| docker run -d nginx:latest                  | Run container in the background     |
|                                             |                                     |
|     **MANAGEMENT OF CONTAINERS**            |                                     |
|                                             |                                     |
| docker stop [ID_CONTAINER]                  | Stop the container                  |
| docker rm [ID_CONTAINER]                    | Delete the container                |
| docker rm -f [ID_CONTAINER]                 | Force deletion of the container     |
| docker rm -f $(docker ps -q)                | Delete all active containers        |
| docker rm -f $(docker ps -qa)               | Delete EVERY container              |




<tr><td align="left"><code>New gist</code></td>                     <td align="left">Ouvrir un nouveau gist. Pour plus d’informations, consultez «&nbsp;<a href="/fr/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists" _originalhref="/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Création de gists</a>&nbsp;».</td></tr>


