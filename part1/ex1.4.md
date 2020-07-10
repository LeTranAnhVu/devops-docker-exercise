
#### command :
```shell script
docker pull devopsdockeruh/exec_bash_exercise
docker run -d --name log-it devopsdockeruh/exec_bash_exercise
docker exec -it log-it bash
# inside container
tail -f logs.txt
```

#### secret message: 
`Docker is easy`