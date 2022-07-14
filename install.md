# 목차
- [목차](#목차)
- [Docker](#docker)
  - [1.1 Docker Doc](#11-docker-doc)
  - [1.2 설치 확인](#12-설치-확인)
  - [1.3 docker hub](#13-docker-hub)
  - [1.4. 명령어](#14-명령어)

# Docker
- Linux OS 

> 다른 OS도 설치 가능

## 1.1 Docker Doc
- https://docs.docker.com/
- [x] Download and install
- [x] OS에 맞게 설치

## 1.2 설치 확인
터미널
```
docker images // window
sudo docker images // mac
```
- 에러가 뜨지 않는다면 정상적으로 설치 완료


## 1.3 docker hub
- https://hub.docker.com/
- docker hub -> images -> container

## 1.4. 명령어

- 컨테이너 생성
```
docker run httpd
docker ps
docker run --name [설치된 이름]
docker stop [컨테이너이름 혹은 아이디]
docker ps -a
docker start // 중지했던 컨테이너 다시 실행
docker logs [컨테이너이름]
docker logs -f [컨테이너이름] 로그 실시간
docker rm [컨테이너이름]
docker rm --force [컨테이너이름] // stop하지 않아도 삭제가능
docker rmi [이름]

docker run -p 80:80 [컨테이너이름]
docker exec [컨테이너이름] pwd
docker exec -it [컨테이너이름] /bin/sh

exit
```

