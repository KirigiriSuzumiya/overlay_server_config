# overlay_server_config
easy using overlay server mainly depened on docker container, serving serveral widely honored opensource self-hosted projects: minio,filestash,onlyoffice,rustdesk...

for Personal usage, may not be widely available.

## How to Use

simply `docker compose-up`, then everything is done!

## Remote File Group
object storage, office viewers and editors and even multi-platform web client:
- [MinIO](https://min.io/) 
    - API on port `9000`, Web Console on port `9090`, FTP service on port `8021`
    - High Performance Object Storage for Modern Data Lakes and Data LakeHouses
    - for me, simply served it as file storage service
- [onlyoffice](https://www.onlyoffice.com/)
    - HTTP service on port `8080`, HTTPS unavailable.
    - free collaborative online office suite comprising viewers and editors for texts, spreadsheets and presentations, forms and PDF
- [filestash](https://www.filestash.app/)
    - Web service on port `80`
    - A modern web client for SFTP, S3, FTP, WebDAV, Git, Minio, LDAP, CalDAV, CardDAV, Mysql, Backblaze, ...
    - for me, I'm using it to connect S3-like MiniIO and it's FTP service.

```shell
cd overlay_server_config/minio-onlyoffice-filestash
docker-compose up
```
    

## Remote Display Protocol Group
- [rustdesk](https://rustdesk.com/)
    - TCP port:`21115-21119`, UDP port:`21116`
    - An open-source remote desktop, and alternative to TeamViewer.
    - Highly recommended on both using an Intranet ip address for direct connection or a overlay server for remote connection
- [rustdesk web client](https://rustdesk.com/)
    - HTTP service on port `5000`
    - Get rid of software client, connect remote device using simply Web UI!

```shell
cd overlay_server_config/rustdesk-server-web
docker-compose up
```