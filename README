#go to https://hub.docker.com/r/jupyter/base-notebook/ 
docker pull jupyter/base-notebook

mkdir mission

cd mission

mkdir mission1

cd mission1

#create a docker-compose.yml file

version: '3'
services:
  mission1:
    image: jupyter/base-notebook
    container_name: mission1-jupyter-notebook
    ports:
      - "8888:8888"
    volumes:
      - ./work:/home/jovyan/work/
    command: start-notebook.sh --NotebookApp.token=''

#make the mapping directory

mkdir work

#use docker compose

docker-compose up -d

#go to your brower and input your localhostIP:8888
