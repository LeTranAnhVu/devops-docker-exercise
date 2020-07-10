
#### command :
```shell script
docker run -it --name read_website ubuntu:16.04 sh -c 'apt-get update; apt-get install -y curl; echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```