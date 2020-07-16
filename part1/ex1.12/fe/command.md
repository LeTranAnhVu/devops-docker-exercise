```shell script
# build the image
docker build -t node_fe .

# run container
docker run -it -p 5000:5000 --name fe_app node_fe
```