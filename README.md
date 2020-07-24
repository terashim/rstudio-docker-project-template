Local Docker RStudio Server Project Template
==================================================

## Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop) for Windows/Mac
    - Docker 18.06+

## Settings

1. Browse [terashim/rstudio-docker-project-template](https://github.com/terashim/rstudio-docker-project-template) and use this template to create a new repository.
2. Clone the repository to your local machine.
3. Edit
    - `_rstudio/Dockerfile`
        - change the base image, install packages, change global options, etc.
    - `_rstudio/docker-compose.yml`
        - rename the image name `your-project-name:latest`
        - rename the folder name to mount `/home/rstudio/your-project-name`
4. Rename `your-project-name.Rproj` file

---

## Usage

1. Start RStudio Server:
    ```sh
    docker-compose up -d
    ```
2. Browse <http://localhost:8787> to connect to the local RStudio Server.
3. Stop the RStudio Server:
    ```sh
    docker-compose down
    ```
