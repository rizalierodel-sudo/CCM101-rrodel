# MinIO Deployment

## Docker Command

The following Docker command was used to deploy the MinIO object storage server:

    docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"

Port 9000 was used for the MinIO API, while port 9001 was used for the MinIO Web Console.

## Web Console Port

The MinIO Web Console was accessed using port 9001 through the KillerCoda port forwarding feature.

## Bucket Created

The storage bucket created during the activity was **client-photos**.

The bucket was used to store the sample file uploaded through the MinIO Web Console.

## Environment Variables

The `-e` flags were used to set the login credentials for the MinIO server.

### MINIO_ROOT_USER

The `MINIO_ROOT_USER` environment variable sets the root username for the MinIO server. In this activity, the username was set to **cloudadmin**.

### MINIO_ROOT_PASSWORD

The `MINIO_ROOT_PASSWORD` environment variable sets the root password for the MinIO server. In this activity, the password was set to **CloudNova2026!**.

## Verification

After running the Docker command, the container was checked using `docker ps`.

The MinIO container was running with ports 9000 and 9001 mapped successfully.

The MinIO Web Console was then accessed through KillerCoda's port forwarding feature. After logging in, the `client-photos` bucket was created and the sample file **MinIO Cloud Storage Test.txt** was uploaded successfully.
