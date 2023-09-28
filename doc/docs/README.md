# 🤗 Welcome to KirigiriSuzumiya's Toolkit server

This is an easy-to-built toolkit overlay server contained various open-sourced tools, deployed by `docker compose-up` 

## 🔗 Fast Link

[docuseak](http://110.42.255.139:3000) | [filestash](http://110.42.255.139:9080) | [minio](http://110.42.255.139:9090) | [rustdesk](http://110.42.255.139:5000) 

## 🗃️ Remote File Group
object storage, office viewers and editors and even multi-platform web client:
- [MinIO](https://min.io/) 
    - API on port `9000`, Web Console on port `9090`, FTP service on port `8021`
    - High Performance Object Storage for Modern Data Lakes and Data LakeHouses
    - for me, simply served it as file storage service
- [onlyoffice](https://www.onlyoffice.com/)
    - HTTP service on port `8080`, HTTPS unavailable.
    - free collaborative online office suite comprising viewers and editors for texts, spreadsheets and presentations, forms and PDF
- [filestash](https://www.filestash.app/)
    - Web service on port `9080`
    - A modern web client for SFTP, S3, FTP, WebDAV, Git, Minio, LDAP, CalDAV, CardDAV, Mysql, Backblaze, ...
    - for me, I'm using it to connect S3-like MiniIO and it's FTP service.
    

## 💻 Remote Display Protocol Group
- [rustdesk](https://rustdesk.com/)
    - TCP port:`21115-21119`, UDP port:`21116`
    - An open-source remote desktop, and alternative to TeamViewer.
    - Highly recommended on both using an Intranet ip address for direct connection or a overlay server for remote connection
- [rustdesk web client](https://rustdesk.com/)
    - HTTP service on port `5000`
    - Get rid of software client, connect remote device using simply Web UI!


## 🗎 Online document filling, signing and site generator

- [DocuSeal](https://github.com/docusealco/docuseal)
    - WEB service on port `3000`
    - DocuSeal is an open source platform that provides secure and efficient digital document signing and processing. 
    - Create PDF forms to have them filled and signed online on any device with an easy-to-use, mobile-optimized web tool.
- [docsify](https://github.com/docsifyjs/docsify/)
    - This page on port `80`
    - Docsify turns one or more Markdown files into a Website, with no build process required.