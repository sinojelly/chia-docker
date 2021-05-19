# Usage

## Build docker image
docker build -t jelly/chia:latest .

## Run docker
```
docker pull sinojelly/chia:latest
docker run -it -v ~/work:/work sinojelly/chia:latest /bin/bash
```

## Plot disk
```
. ./activate
chia init
chia plots create -k 10 -f 0x1234 -p 0x1234 -t /work/tmp -2 /work/tmp2 -d /work/result
```
测试用的命令行：
```
 chia plots create --override-k -k 25 -f 875c6b53658e8bb2f22a250efa74ee7d034f386db9bd2a74a9f2db97afd47edf8f92e8a796fedf47d731bd04407c697f -p 8777383e870433183cbee0ce6b9ad30877e32aa63c6b654b95634ff75ac2f5d8606cd188dc294bf0c07df33d879f603c -t /work/tmp -2 /work/tmp2 -d /work/result
```

## chia command line helper
```
chia -h
chia plots -h
chia plots check -h
chia start -h
```
