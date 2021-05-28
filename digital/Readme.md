## Digital Ocean POC
- Connect to instance: `ssh root@165.227.222.50 -i ~/.ssh/id_rsa`
- Userdata
```
sudo apt-get update
sudo apt-get remove docker docker-engine docker.io
sudo apt install docker.io
sudo apt  install docker-compose
sudo systemctl start docker
sudo systemctl enable docker

# download docker-compose.yml

docker-compose 
```
