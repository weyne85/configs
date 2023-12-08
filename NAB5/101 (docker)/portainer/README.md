### Installation

## Create Volume for Portainer
docker volume create portainer_data

## Download and install Portainer
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest

# Log in
Visit: https://localhost:9443