## PSUSphere Docker

### Project Description

PSUSphere is a Django web application packaged using Docker. Docker allows the application to run in a consistent environment across different machines without requiring manual installation of all Python dependencies.

## Instructional Procedure

Before running the application, make sure you have installed:

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- Docker Compose (included with Docker Desktop)
- A Docker Hub account to access or publish the image

## Build and Run Locally

1. Clone or download the project repository.
2. Open PowerShell in the project root directory, where the `Dockerfile` and `docker-compose.yml` are located.
3. Build the Docker image:

   ```powershell
   docker compose build
   ```

4. Start the application:

   ```powershell
   docker compose up -d
   ```

5. Open the application in your browser:

   http://localhost:8000

To view the container status:

```powershell
docker compose ps
```

To view application logs:

```powershell
docker compose logs
```

To stop the application:

```powershell
docker compose down
```

## Docker Hub Image

The Docker image is published to Docker Hub under the following name:

`janepauline/psusphere-docker:latest`


## Pull and Run the Docker Hub Image

1. Make sure Docker Desktop is running.
2. Open PowerShell in a folder containing the client `docker-compose.yml` file.
3. Pull the image from Docker Hub:

   ```powershell
   docker janepauline/psusphere-docker:latest
   ```

4. Start the application using the client configuration:

   ```powershell
   docker compose up -d
   ```

5. Open the application:

   http://localhost:8000

To stop the application:

```powershell
docker compose down
```
