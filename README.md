```
docker-compose up -d --build
docker-compose exec web service ssh start

docker-compose exec workstation bash

# In de container
ssh -p 999 sshuser@web

```