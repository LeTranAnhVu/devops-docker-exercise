#youtube-dl
[Docker-hub link](https://hub.docker.com/r/letrananhvu/youtube-dl)

#### Usage: 
- A docker container uses for downloading youtube video.
   
#### clone:
`
docker pull letrananhvu/youtube-dl
`

#### run container:
`
docker run --name youtube-downloader -v $(pwd):/mydir letrananhvu/youtube-dl <link>
`
- replace `<link>` with the url of youtube video.