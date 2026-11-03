## To Pull and Run newer images:
```bash
docker pull mosesmbadi/hl7-astm-parser:latest

docker stop lis-server
docker rm lis-server

docker run -d --name lis-server -p 9091:9091 --restart unless-stopped mosesmbadi/hl7-astm-parser:latest
```


Or if strictly on compose terms


```docker compose pull lis_server && docker compose up -d --no-deps lis_server```