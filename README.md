```bash
docker build -f server/Dockerfile -t cors-server
docker build -f client/Dockerfile -t cors-client
docker network create cors
docker run -p 3000:3000 -d --name cors-server --network cors cors-server
docker run -p 8080:80 -d --name cors-client --network cors cors-client
```