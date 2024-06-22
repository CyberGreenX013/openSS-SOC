## Shuffle:
https://github.com/shuffle/shuffle/blob/main/.github/install-guide.md#after-installation
Step 1:
https://docs.docker.com/engine/install/
Step 2:
git clone https://github.com/Shuffle/Shuffle
cd Shuffle
docker compose up -d
docker ps

docker logs 734269c4a547 --follow (shuffle-backend)

sudo chown -R 1000:1000 shuffle-database
sudo sysctl -w vm.max_map_count=262144
sudo docker restart shuffle-opensearch

#if shuffle app not direct download
##Locatin ./Shuffle/
git clone https://github.com/shuffle/python-apps

sudo rm /etc/apt/sources.list.d/docker.list