```shell script
# build the image
docker build -t node_img .

# run container
docker run -it -p 5000:5000 --name node_con node_img
```