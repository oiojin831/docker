# docker
Docker
Dockerfile은 Docker Image를 만드는 명세일뿐이다.

Docker-compose는 여러개의 image를 여러개의 container로 한거번에 관리해주는
툴이다

Docker-cleanup는 image랑 container날려주는거다.

image -> class, container -> instance
Dockerfile은 class 코드라고 보면된다.


## docker comman
docker run

## Create rails project
## suspender같은 시작 프로젝트 만드는 스크립트
docker pull rails
docker run -it --rm --user $(id -u):$(id -g) -v $PWD:/usr/src/app -w
/usr/src/app rails rails new --skip-bundle mobydock
docker run -it --rm --user "$(id -u):$(id -g)" -v "$PWD":/usr/src/app -w
/usr/src/app rails rails new --skip-bundle mobydock
새로운 docker container를 만들어서 이유저와 이 위치에서 rails image로 rails
command를 실행 시키고 container를 없앤다.

필요한 설정 파일들을 github에서 wget으로 가져온
docker도 가져온다.

