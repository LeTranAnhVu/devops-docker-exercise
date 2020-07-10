```shell script
#create logs.txt file in local machine (mac osx)
touch logs.txt
# start logging
docker run -v $(pwd)/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
```