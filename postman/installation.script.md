## Deploy on ubuntu machine 

#### Script 
```shell

## enter into docker ubuntu terminal
docker run -it --name bookerservice -p 3001:80 ubuntu /bin/bash

apt update 
apt install git
cd /var
mkdir www
apt install curl

## Install nvm 
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
nvm install 16 

git clone https://github.com/keshav-repo/restful-booker.git

docker exec -it  bookerservice /bin/bash

apt update
apt install nginx
service nginx status

apt update
apt install vim

## command to check ip address of running docker ubuntu container 
docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' bookerservice

docker container update --publish-add 3001:80 bookerservice

/etc/systemd/system

systemctl daemon-reload

bash: systemctl: command not found
apt-get install systemd

sudo systemctl enable booking.service 

sudo chmod 664 

sudo systemctl start booking.service 

ps ef | grep node 

nohup npm run start > output.log 2>&1 &

newman run Booking2.postman_collection.json -e dev.postman_environment.json


sudo ln -s /home/keshavnit16/.nvm/versions/node/v16.20.2/bin/newman

/home/keshavnit16/.nvm/versions/node/v16.20.2/bin/newman    

sudo systemctl status jenkins

newman run postman/Booking.postman_collection.json -e postman/dev.postman_environment.json

```

#### NGINX test
```shell 

docker run -it --name nginxtest -p 80:80 ubuntu /bin/bash

apt-get update
apt-get install ufw


apt-get install sudo

docker run --name docker-nginx -p 80:80 nginx

docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' docker-nginx
```

#### Jenkins 

docker run -it --name jenkinstest -p 3002:80 ubuntu /bin/bash


