# 목차
- [목차](#목차)
- [1. container](#1-container)
  - [1.1 VM](#11-vm)
  - [1.2. Container Engine](#12-container-engine)
  - [1.3. Building Containers](#13-building-containers)
    - [1.3.1. Dockerfile(설명서)](#131-dockerfile설명서)
    - [1.3.2. Image](#132-image)
    - [1.3.3. Container](#133-container)
  - [1.4. Shipping Containers](#14-shipping-containers)
  - [1.5. 명령어](#15-명령어)

# 1. container
- 에플리케이션을 구동하기 위한 모든 것들을 담은 패키징 툴

## 1.1 VM
- Hypervisor(vmware, VirtualBox)를 이용하여 가상의 머신을 만들 수 있다.
- 한 운영체제 위에 동일한 어플리케이션을 구동
- 무거운 운영체제를 포함함
- 운영체제의 리소스를 잡아 먹는 범인이 될 수 있다.

## 1.2. Container Engine
- 운영체제를 포함하지 않고 container engine 설치된 host os를 공유
- 가장 많이 사용하는 docker

## 1.3. Building Containers
### 1.3.1. Dockerfile(설명서)
- copy files
- install dependencies
- set environment variables
- run setup scripts
### 1.3.2. Image
- 실행되고 있는 어플리케이션을 상태를 스냅샷하여 이미지를 만들어놓는다고 생각하면 쉽다.
- 불변의 상태
- Dockerfile, configuration 등등
### 1.3.3. Container
- 컨테이너 안에서 우리의 이미지를 이용해서 어플리케이션을 구동

## 1.4. Shipping Containers
![image](https://user-images.githubusercontent.com/71534090/187482167-5c60007c-bfcc-438c-adb7-bfd29bc33ef9.png)


## 1.5. 명령어

```shell
docker build -f Dockerfile -t [도커이미지 이름부여] .
doker images
docker run -d -p hostPort:containerPort [도커미이지 이름]
docker ps
docker logs [컨테이너ID]

docker push 계정명/repository:tagname
docker tag [기존명] [변경명]
```
