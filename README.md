# nginx-octo-fiesta

### Copy configuration files if necessary
```bash
nginx docker cp $(docker ps -q):/etc/nginx .
```
### Stop current container
```bash
docker stop $(docker ps -q)
```
### Start container and build
```bash
docker compose up --build
```
### Access container running bash
```bash
docker exec -it $(docker ps -q) bash
```