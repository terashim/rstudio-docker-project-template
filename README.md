Local Docker RStudio Server Project Template
==================================================

## Settings

Edit

- `_rstudio/Dockerfile`
    - change the base image, install packages, change global options, etc.
- `_rstudio/docker-compose.yml`
    - rename the image name `your-project-name:latest`
    - rename the folder name to mount `/home/rstudio/your-project-name`

Rename `your-project-name.Rproj` file

---

## Usage

1. Start RStudio Server:
    ```sh
    docker-compose up
    ```
2. Browse <http://localhost:8787> to connect to the local RStudio Server.
3. Stop the RStudio Server:
    ```sh
    docker-compose down
    ```
