# MinIO Deployment

## Deploying MinIO with Docker

The MinIO server was deployed using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

The `-d` option runs the MinIO container in detached mode so it can continue running in the background.

The `--name minio-server` option gives the container a specific name that can be used when managing it with Docker commands.

## Port Configuration

Two ports were mapped:

| Port | Purpose |
|---|---|
| 9000 | MinIO API port |
| 9001 | MinIO Web Console |

Port **9001** was used to access the MinIO Web Console through the KillerCoda port forwarding feature.

## Environment Variables

The `-e` flags set environment variables inside the MinIO container.

```bash
-e "MINIO_ROOT_USER=cloudadmin"
```

This sets the root username used to log in to the MinIO server.

```bash
-e "MINIO_ROOT_PASSWORD=CloudNova2026!"
```

This sets the root password for the MinIO server.

## Bucket Created

The storage bucket created during the activity was:

```text
client-photos
```

A sample file was uploaded to the bucket to verify that the object storage system was working correctly.

## Verification

The MinIO container was verified using:

```bash
docker ps
```

The MinIO Web Console was then accessed through port `9001`, where the `client-photos` bucket and uploaded file were confirmed.
