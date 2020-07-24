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

Start RStudio server:

```sh
docker-compose up
```

Open <http://localhost:8787>

Stop RStudio Server:

```sh
docker-compose down
```
