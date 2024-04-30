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




<table><thead><tr><th align="left" scope="col">Commande</th><th align="left" scope="col">Comportement</th></tr></thead><tbody><tr><td align="left"><code>Import repository</code></td><td align="left">Créer un dépôt en important un projet à partir d’un autre système de gestion de versions. Pour plus d’informations, consultez «&nbsp;<a href="/fr/migrations/importing-source-code/using-github-importer/importing-a-repository-with-github-importer" _originalhref="/migrations/importing-source-code/using-github-importer/importing-a-repository-with-github-importer" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Importation d’un dépôt avec GitHub Importer</a>&nbsp;».</td></tr><tr><td align="left"><code>New gist</code></td><td align="left">Ouvrir un nouveau gist. Pour plus d’informations, consultez «&nbsp;<a href="/fr/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists" _originalhref="/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Création de gists</a>&nbsp;».</td></tr><tr><td align="left"><code>New organization</code></td><td align="left">Créer une organisation. Pour plus d’informations, consultez «&nbsp;<a href="/fr/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch" _originalhref="/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Création d’une organisation à partir de zéro</a>&nbsp;».</td></tr><tr><td align="left"><code>New project</code></td><td align="left">Créer un nouveau projet. Pour plus d’informations, consultez «&nbsp;<a href="/fr/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project" _originalhref="/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Création d’un project</a>&nbsp;».</td></tr><tr><td align="left"><code>New repository</code></td><td align="left">Créer un dépôt à partir de zéro. Pour plus d’informations, consultez «&nbsp;<a href="/fr/repositories/creating-and-managing-repositories/creating-a-new-repository" _originalhref="/repositories/creating-and-managing-repositories/creating-a-new-repository" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Création d’un dépôt</a>&nbsp;».</td></tr><tr><td align="left"><code>Switch theme to &lt;theme name&gt;</code></td><td align="left">Passer directement à un autre thème pour l’interface utilisateur. Pour plus d’informations, consultez «&nbsp;<a href="/fr/get-started/accessibility/managing-your-theme-settings" _originalhref="/get-started/accessibility/managing-your-theme-settings" aria-roledescription="Pointer la carte" aria-describedby="popover-describedby">Gestion de vos paramètres de thème</a>&nbsp;».</td></tr></tbody></table>

| Commande              | Comportement                                                                                                                                                                  |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `Import repository`   | Créer un dépôt en important un projet à partir d’un autre système de gestion de versions. Pour plus d’informations, consultez [Importation d’un dépôt avec GitHub Importer](https://docs.github.com/fr/github/importing-your-projects-to-github/importing-a-repository-with-github-importer). |
| `New gist`            | Ouvrir un nouveau gist. Pour plus d’informations, consultez [Création de gists](https://docs.github.com/fr/github/writing-on-github/editing-and-sharing-content-with-gists/creating-gists).                                        |
| `New organization`    | Créer une organisation. Pour plus d’informations, consultez [Création d’une organisation à partir de zéro](https://docs.github.com/fr/github/setting-up-and-managing-your-github-user-account/creating-an-organization-from-scratch).    |
| `New project`         | Créer un nouveau projet. Pour plus d’informations, consultez [Création d’un projet](https://docs.github.com/fr/github/managing-your-work-on-github/planning-and-tracking-your-work-with-issues-and-projects/creating-a-project).               |
| `New repository`      | Créer un dépôt à partir de zéro. Pour plus d’informations, consultez [Création d’un dépôt](https://docs.github.com/fr/github/getting-started-with-github/quickstart/create-a-repo).                                                      |
| `Switch theme to <theme name>` | Passer directement à un autre thème pour l’interface utilisateur. Pour plus d’informations, consultez [Gestion de vos paramètres de thème](https://docs.github.com/fr/github/setting-up-and-managing-your-github-profile/managing-your-theme-settings). |


