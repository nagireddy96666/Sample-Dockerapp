docker rm -f $(docker ps -a -q)
docker rmi $(docker images -q)
sudo docker build -t my-flask-app .
sudo docker run -p 8000:5000 my-flask-app
sudo netstat -tuln | grep 8080
sudo docker run -p 8080:5000 my-flask-app
sudo docker exec -it nervous_aryabhata /bin/bash
