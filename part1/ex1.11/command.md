```shell script
# build the image
docker build -t my_node_be .

# create logs.txt in host machine
touch logs.txt

# run container
docker run -it -p 8000:8000 -v $(pwd)/logs.txt:/backend-example-docker/logs.txt --name my_be my_node_be
```