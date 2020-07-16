```shell script
#build img
docker build -t ex113 .

#run container
docker run --name java_app -p 8080:8080 ex113
```