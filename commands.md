***Cria um imagem***
sudo docker build -t sample:dev .

***Rodar Container***
docker run -v ${PWD}:/app -v /app/node_modules -p 3001:3000 --rm sample:dev


***Container inside Container****
podman run --privileged -it localhost/fedora_podman
docker run --privileged -it fedora

podman run -it --privileged ubuntu-podman

podman run -p 3000:3000 --rm react

***Lista todos os container ****
docker ps -a 

***Apaga uma imagem****
sudo docker rmi 8eeadf3757f4

***Apaga uma container***
docker rm -f f0e0e8cf43df-

***Delete all conainers***
podman system prune

*** delete all images****
sudo podman image prune --all

***rodar container e acessar o terminal***
sudo docker run -it image-react bash


***rodar container e acessar o terminal***
sudo docker run -it -p 3000:3000 -d image-react npm start





