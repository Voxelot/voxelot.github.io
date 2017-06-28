Common Docker Commands
===

```
# Clean all images by name
docker rmi -f $(docker images | grep 'IMAGE_NAME' | tr -s ' ' | cut -d ' ' -f 3)

# Delete all stopped containers
docker rm $( docker ps -q -f status=exited)

```
