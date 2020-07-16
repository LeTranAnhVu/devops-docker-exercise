```shell script
# build the image
docker build -t node_be .

# run container
docker run -it -p 8000:8000 --name be_app node_be
```