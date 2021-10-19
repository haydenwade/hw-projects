## Digital Ocean POC
- Connect to instance: `ssh root@165.227.222.50 -i ~/.ssh/id_rsa`
- Userdata
```
sudo apt-get update
sudo apt-get remove docker docker-engine docker.io
sudo apt install docker.io docker-compose git nodejs npm nginx python3-certbot-nginx
sudo systemctl start docker
sudo systemctl enable docker

git clone https://github.com/haydenwade/hw-projects.git

cd hw-projects/digitalocean
docker-compose up -d
```


sudo certbot --nginx -d teamwawe.com -d www.teamwawe.com
sudo certbot --nginx -d zeroplusonepodcast.com -d www.zeroplusonepodcast.com
sudo certbot --nginx -d haydenwade.com -d www.haydenwade.com


## Apps
- haydenwade.com - port: 3000
- zeroplusonepodcast.com - port: 3001
- teamwawe.com - port: 3002

## Deploying new changes
- `docker-compose pull`
- `docker-compose up -d`