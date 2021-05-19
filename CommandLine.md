# Usage

## Build docker image
docker build -t jelly/chia:latest .

## Run docker
docker run -it -v ~/work:/work jelly/chia:latest /bin/bash

## Plot disk
```
chia plots create -k 10 -f 0x1234 -p 0x1234 -t /work/tmp -2 /work/tmp2 -d /work/result
```


## chia command line helper
```
chia -h
chia plots -h
chia plots check -h
chia start -h
```
