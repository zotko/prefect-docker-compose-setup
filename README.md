# Prefect Docker-Compose Setup

This `docker-compose.yml` file sets up a local Prefect environment using Prefect version `2.19.7`. It includes services for PostgreSQL, MinIO, Prefect Server, and Prefect Worker (Docker).

## Setup Instructions

1. Create a `.env` file with the following content:

   ```env
   BASE_URL=http://localhost
   POSTGRES_USER=your_user
   POSTGRES_PASSWORD=your_password
   MINIO_ROOT_USER=your_user
   MINIO_ROOT_PASSWORD=your_password
   ```

2. Start the services:

   ```sh
   docker-compose up -d
   ```

3. Access the services:
   - Prefect Server UI: `http://localhost:4200`
   - MinIO Console: `http://localhost:9001`

4. Stop the services:

   ```sh
   docker-compose down
   ```

5. Clean up:

   ```sh
   docker-compose down -v
   ```