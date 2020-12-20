# Delete containers & images
```bash
# Get all container IDs
docker container ls -aq
# Delete all containers with filters that match a label
docker container prune ––filter=”label==maintainer=Jeremy”
# Delete all containers with filters that don't match a label
docker container prune ––filter=”label!=maintainer=Jeremy”
# Delete all containers
docker container rm $(docker container ls -aq)
```