## To Pull and Run newer images:
```bash
docker pull mosesmbadi/hl7-astm-parser:latest

docker stop lis-server
docker rm lis-server

docker run -d --name lis-server -p 9091:9091 --restart unless-stopped mosesmbadi/hl7-astm-parser:latest
```