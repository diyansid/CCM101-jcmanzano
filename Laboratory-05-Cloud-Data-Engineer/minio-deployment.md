# MinIO Object Storage Deployment

## Overview

For this laboratory activity, I deployed MinIO Object Storage using Docker in the KillerCoda Linux environment. MinIO provides S3-compatible object storage for files such as images, videos, backups, documents, and application data.

## Docker Environment

Before deploying MinIO, I verified that Docker was installed and running.

Commands used:

- docker --version
- docker ps

Docker version 29.1.3 was available in the KillerCoda environment.

## MinIO Deployment

MinIO was deployed as a Docker container using the following configuration:

- Container name: minio
- API port: 9000
- Web Console port: 9001
- Docker image: quay.io/minio/minio
- Data directory: /data

The container was started using Docker and the MinIO image was downloaded successfully.

## Port Configuration

Two ports were configured for MinIO:

- Port 9000 - MinIO API
- Port 9001 - MinIO Web Console

The MinIO logs confirmed that both the API and WebUI were running.

## Object Storage Bucket

After opening the MinIO Web Console, I created a private bucket named `client-photos`.

I then uploaded an image into the bucket to demonstrate object storage. The uploaded object appeared successfully inside the `client-photos` bucket.

## Verification

I verified the deployment using the `docker ps` command. The container named `minio` displayed an Up status with ports 9000 and 9001 exposed.

## Result

The MinIO deployment was successful. I was able to deploy an object storage server using Docker, access its web interface, create a private bucket, and upload an object. This activity demonstrated how object storage can be deployed and managed in a practical cloud-like environment.

## Exact Docker Command Used

The exact Docker command I used for the MinIO deployment was:

    docker run -d \
      --name minio \
      -p 9000:9000 \
      -p 9001:9001 \
      -e MINIO_ROOT_USER=admin \
      -e MINIO_ROOT_PASSWORD=admin12345 \
      quay.io/minio/minio server /data --console-address ":9001"

## Environment Variables

The `-e` flags in the Docker command are used to define environment variables inside the container.

- `MINIO_ROOT_USER=admin` configured the administrator username used to log in to MinIO.
- `MINIO_ROOT_PASSWORD=admin12345` configured the administrator password.

Environment variables allow configuration values to be passed to the container when it starts without modifying the MinIO application itself.

## Web Console and Bucket

The MinIO Web Console was accessed through **port 9001**.

The object storage bucket created for the activity was named **client-photos**. A sample image was successfully uploaded to this bucket.
