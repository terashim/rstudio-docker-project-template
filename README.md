Local Docker RStudio Server Project Template
==================================================

## Settings

Edit

- `Dockerfile`
- `docker-compose.yml`
    - `PROJECT_RSTUDIO_IMAGE`
    - `PROJECT_NAME`

Rename `PROJECT_NAME.Rproj`

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
