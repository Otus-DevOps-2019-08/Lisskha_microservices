# Lisskha_microservice repository by Yuliya Kharchenko

## Table of contents
- [HW12. Docker: Введение](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-12-docker-введение)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2)
- [HW13. Docker: Микросервисы](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/blob/master/README.md#hw-13-docker-%D0%BC%D0%B8%D0%BA%D1%80%D0%BE%D1%81%D0%B5%D1%80%D0%B2%D0%B8%D1%81%D1%8B)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-1)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-1)
- [HW14. Docker: Network, docker-compose](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-14-docker-network-docker-compose)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-2)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-2)
- [HW15. Gitlab CI: Построение процесса непрерывной поставки](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-15-gitlab-ci-%D0%BF%D0%BE%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81%D0%B0-%D0%BD%D0%B5%D0%BF%D1%80%D0%B5%D1%80%D1%8B%D0%B2%D0%BD%D0%BE%D0%B8%CC%86-%D0%BF%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BA%D0%B8)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-3)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-3)
- [HW16. Введение в мониторинг]()
    - [Доп. задание №1]()
    - [Доп. задание №2]()

# HW 12. Docker: Введение

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/1/files

- Установлены:
```sh
$ docker version
Client: Docker Engine - Community
 Version:           19.03.1
 API version:       1.40
 Go version:        go1.12.5
 ...
Server: Docker Engine - Community
 Engine:
  Version:          19.03.1
  API version:      1.40 (minimum version 1.12)
  Go version:       go1.12.5

$ docker-compose -v
docker-compose version 1.24.1, build 4667896b

$ docker-machine -v
docker-machine version 0.16.1, build cce350d7
```
- Запуск конта:
```sh
$ docker run hello-world
...
Hello from Docker!
```
- Список контов:
```sh
$ docker ps -a
```
- Список имиджей:
```sh
$ docker images
```
- Запуск и вход внутрь конта:
```sh
$ docker run -it ubuntu:16.04 /bin/bash
```
- **docker run** запускает новый конт каждый раз
- Если флаг **--rm**, то после остановки конта, содержимое будет удалено с диска
- Работа с **docker ps**
```sh
$ docker ps -a --format "table {{.ID}}\t{{.Image}}\t{{.CreatedAt}}\t{{.Names}}"
CONTAINER ID        IMAGE               CREATED AT                      NAMES
c6fcb5db6c5b        ubuntu:16.04        2019-11-19 00:27:04 +0300 MSK   musing_davinci
```
- Запуск созданного конта
```sh
$ docker start c6fcb5db6c5b
```
- Присоединить терминал к созданному конту
```sh
$ docker attach c6fcb5db6c5b
```
- 
```sh
docker run = docker create + docker start + docker attach
```
- **docker create** юзается, если не надо стартовать конт сразу после создания

### Docker run
- Через параметры передаются лимиты(cpu/mem/disk), ip, volumes  
*-i* – запускает контейнер в foreground режиме (docker attach)  
*-d* – запускает контейнер в background режиме  
*-t* - создает TTY  
*docker run -it ubuntu:16.04 bash*  
*docker run -dt nginx:latest*
### Docker exec
- Запускает новый процесс внутри контейнера
```sh
docker exec -it <u_container_id> bash
```
### Docker commit
- Создает image из контейнера
- Контейнер при этом остается запущенным
```sh
$ docker commit c6fcb5db6c5b jull/ubuntu-tmp-file
$ docker images
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
jull/ubuntu-tmp-file   latest              cd948fb78b1e        9 seconds ago       123MB
```

## Доп. задание №1
- Информация о контейнере
```sh
$ docker inspect c6fcb5db6c5b
```
- Информация об имидже
```sh
$ docker inspect 5f2bf26e3524
```
- Описание отличий контейнера и образа в файле docker-monolith/docker-1.log

### Docker kill & stop
- **kill** сразу посылает SIGKILL
- **stop** посылает SIGTERM, и через 10 секунд посылает SIGKILL
- **SIGTERM** - сигнал остановки приложения 
- **SIGKILL** - безусловное завершение процесса
```sh
$ docker ps -q
c6fcb5db6c5b
$ docker kill $(docker ps -q)
c6fcb5db6c5b
```
### Docker system df
- Отображает сколько дискового пространства занято образами, контейнерами и volume’ами
- Отображает сколько из них не используется и возможно удалить
```sh
$ docker system df
```
### Docker rm & rmi
- **rm** - удаляет контейнер, можно добавить флаг **-f**, чтобы удалялся работающий container
- **rmi** удаляет image, если от него не зависят запущенные контейнеры
```sh
$ docker rm $(docker ps -a -q)
fb9e81c240cf
c6fcb5db6c5b
```
```sh
$ docker rmi $(docker images -q)
Untagged: jull/ubuntu-tmp-file:latest
Deleted: sha256:cd948fb78b1e621df8fed21133b738d404b6c554962f72891e5a06f1824ca59a
...
```

## Docker контейнеры. GCE.
- Создала новый проект
- На своей машине:
```sh
gcloud init
gcloud auth application-default login
```
### Docker machine
- **docker-machine** - встроенный в докер инструмент для создания хостов и установки на них docker engine. Имеет поддержку облаков и систем виртуализации (Virtualbox, GCP и др.)  

**Команда создания:** 
```sh
docker-machine create <имя>
```
**Переключение между именами:**
```sh
eval $(docker-machine env <имя>)
```
**Переключение на локальный докер:**
```sh
eval $(docker-machine env --unset)
```
**Удаление**
```sh
docker-machine rm <имя>
```
- **docker-machine** создает хост для докер демона с указываемым образом в *--google-machine-image*. Образы, которые используются для построения докер контейнеров, к этому никак не относятся.
- Все докер команды, которые запускаются в той же консоли после *eval $(docker-machine env <имя>)* работают с удаленным докер демоном в GCP.  

```sh
$ export GOOGLE_PROJECT=docker-259422

$ docker-machine create --driver google \
--google-machine-image https://www.googleapis.com/compute/v1/projects/ubuntu-os-cloud/global/images/family/ubuntu-1604-lts \
--google-machine-type n1-standard-1 \
--google-zone europe-west1-b \
docker-host

...
Docker is up and running!
```
- Проверяем, что наш Docker-хост успешно создан:
```sh
$ docker-machine ls
NAME          ACTIVE   DRIVER   STATE     URL                       SWARM   DOCKER     ERRORS
docker-host   -        google   Running   tcp://35.240.64.47:2376           v19.03.5

$ eval $(docker-machine env docker-host)
```

Отличия вывода команд:
```sh
docker run --rm -ti tehbilly/htop
```
Выводит только PID 1, с которым запущен htop (т.е. процессы в неймспейсе конта)
```sh
docker run --rm --pid host -ti tehbilly/htop
```
Выводит процессы хостовой машины, на которой запущен докер (т.е. процессы неймспейса хостовой машины)  

- Создала в каталоге docker-monolith файлы:
  - [mongod.conf](https://gist.githubusercontent.com/Lisskha/790957b5e3b103fcae09a02626f6de25/raw/98e76c1d9084f37e05d9f37d17f8b0a6b0124d65/mongod.conf) - конфиг для mongodb
  - [start.sh](https://gist.githubusercontent.com/Lisskha/790957b5e3b103fcae09a02626f6de25/raw/98e76c1d9084f37e05d9f37d17f8b0a6b0124d65/start.sh) - скрипт запуска приложения
  - [db_config](https://gist.githubusercontent.com/Lisskha/790957b5e3b103fcae09a02626f6de25/raw/98e76c1d9084f37e05d9f37d17f8b0a6b0124d65/db_config) - переменная окружения со ссылкой на mongodb
  - [Dockerfile](https://gist.githubusercontent.com/Lisskha/790957b5e3b103fcae09a02626f6de25/raw/98e76c1d9084f37e05d9f37d17f8b0a6b0124d65/Dockerfile) - текстовое описание образа

- Сборка образа (запускается в каталоге docker-monolith)
```sh
docker build -t reddit:latest .
```
*-t* - тег для собранного образа
- Смотреть все образы:
```sh
$ docker images -a
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
reddit              latest              4e8932235b85        23 minutes ago      692MB
<none>              <none>              b19e58d2fdb5        23 minutes ago      692MB
<none>              <none>              f92db4a5c445        23 minutes ago      692MB
...
```
- Запуск контейнера и проверка результата:
```sh
$ docker run --name reddit -d --network=host reddit:latest

5a8623f5c010f0adaa3b64dac44646ebd10452ec20c4a1d33cd7a77ded49e2d4

$ docker ps -a
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS               NAMES
5a8623f5c010        reddit:latest       "/start.sh"              10 seconds ago      Up 8 seconds                            reddit

$ docker-machine ls
NAME          ACTIVE   DRIVER   STATE     URL                       SWARM   DOCKER     ERRORS
docker-host   *        google   Running   tcp://35.240.64.47:2376           v19.03.5
```
- Добавила правило для фаерволла:
```sh
$ gcloud compute firewall-rules create reddit-app \
--allow tcp:9292 \
--target-tags=docker-machine \
--description="Allow PUMA connections" \
--direction=INGRESS
```
- Проверка  
http://35.240.64.47:9292/

### Docker Hub
**[Docker hub](https://hub.docker.com/)** - облачный registry сервис от компании Docker  
- Аутентифицировалась на докер хаб:
```sh
$ docker login
...
Login Succeeded
```
- Протегировала и запушила свой образ в докер хаб:
```sh
$ docker tag reddit:latest <my-login>/otus-reddit:1.0
$ docker push <my-login>/otus-reddit:1.0
```
- Скачала и запустила образ на локальной тачке:
```sh
$ docker run --name reddit -d -p 9292:9292 <my-login>/otus-reddit:1.0

$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
<my-login>/otus-reddit   1.0                 4e8932235b85        54 minutes ago      692MB

$ docker ps -a
CONTAINER ID        IMAGE                   COMMAND             CREATED              STATUS              PORTS                    NAMES
40f026f1ba90        <my-login>/otus-reddit:1.0   "/start.sh"         About a minute ago   Up About a minute   0.0.0.0:9292->9292/tcp   reddit
```
- Проверка  
http://localhost:9292/

- **Команды:**
```sh
# Смотреть логи конта
$ docker logs 40f026f1ba90 -f

# Зайти в конт
$ docker exec -it 40f026f1ba90 bash
    ps aux
    # Убить контейнер
    killall5 1

# Проверить что конт стопнулся
$ docker ps -a
    STATUS - Exited

# Стартануть конт и проверить что он запустился
$ docker start 40f026f1ba90 && docker ps -a

# Остановить и удалить конт
$ docker stop 40f026f1ba90; docker rm 40f026f1ba90

# Запуск конта без запуска приложения
$ docker run --name reddit --rm -it <my-login>/otus-reddit:1.0 bash

# Смотреть инфу об образе
$ docker inspect 4e8932235b85

# Смотреть куски информации
$ docker inspect 4e8932235b85 -f '{{.ContainerConfig.Cmd}}'
[/bin/sh -c #(nop)  CMD ["/start.sh"]]

# Запуск конта с приложением из образа (по image id)
$ docker run --name reddit -d -p 9292:9292 4e8932235b85

29eed99a817e4b2a77492cf71dd762d373e4f90eea28efaaa458c155970997ee

# Зайти в конт, добавить/удалить файлы/каталоги
$ docker exec -it reddit bash
    mkdir /test111 && touch test111/test.txt
    rmdir opt/

# Посмотреть внесенные изменения
$ docker diff 29eed99a817e

# Пересоздать конт и проверить что изменения не сохранились
$ docker stop reddit && docker rm reddit && docker run --name reddit --rm -it 4e8932235b85 bash -c ls
```

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)

# HW 13. Docker: Микросервисы

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/2

```
$ brew install hadolint
$ docker-machine ls
$ eval $(docker-machine env docker-host)
$ wget https://github.com/express42/reddit/archive/microservices.zip
$ unzip reddit-microservices.zip && mv reddit-microservices src
```
Приложение состоит из:
- ***post-py*** - сервис, отвечающий за написание постов
- ***comment*** - сервис, отвечающий за написание комментов
- ***ui*** - веб-интерфейс, работающий с другими сервисами  

Созданы файлы:
- [post-py/Dockerfile](https://gist.githubusercontent.com/Lisskha/dacfa1f77ace3b6e7936c6d1ac914399/raw/764cc60ae3761e783a9dd3607d72c0c5e165d592/post-py%2520Dockerfile)
- [comment/Dockerfile](https://gist.githubusercontent.com/Lisskha/dacfa1f77ace3b6e7936c6d1ac914399/raw/764cc60ae3761e783a9dd3607d72c0c5e165d592/comment%2520Dockerfile)
- [ui/Dockerfile](https://gist.githubusercontent.com/Lisskha/dacfa1f77ace3b6e7936c6d1ac914399/raw/764cc60ae3761e783a9dd3607d72c0c5e165d592/ui%2520Dockerfile)

Скачала последнюю версию образа MongoDB:
```sh
$ docker pull mongo:latest
```
Собрала образы с сервисами:
```sh
$ docker build -t <my_dockerhub_login>/post:1.0 ./post-py
$ docker build -t <my_dockerhub_login>/comment:1.0 ./comment
$ docker build -t <my_dockerhub_login>/ui:1.0 ./ui

$ docker images
REPOSITORY                         TAG                 IMAGE ID            CREATED             SIZE
<my_dockerhub_login>/ui            1.0                 be26bf2af4d7        13 minutes ago      783MB
<my_dockerhub_login>/comment       1.0                 5e14a8dbea9d        15 minutes ago      781MB
<my_dockerhub_login>/post          1.0                 d9b9efa647df        17 minutes ago      117MB
```
Создала сеть для приложения и запустила конты:
```sh
$ docker network create reddit
$ docker run -d --network=reddit --network-alias=post_db --network-alias=comment_db mongo:latest
$ docker run -d --network=reddit --network-alias=post <my_dockerhub_login>/post:1.0
$ docker run -d --network=reddit --network-alias=comment <my_dockerhub_login>/comment:1.0
$ docker run -d --network=reddit -p 9292:9292 <my_dockerhub_login>/ui:1.0
```

Проверка
http://35.195.116.154:9292/

- Оптимизировала и пересобрала образ для [ui](https://gist.githubusercontent.com/Lisskha/dacfa1f77ace3b6e7936c6d1ac914399/raw/764cc60ae3761e783a9dd3607d72c0c5e165d592/ui%2520Dockerfile%2520new):
```sh
$ vim ui/Dockerfile
$ docker build -t <my_dockerhub_login>/ui:2.0 ./ui
$ docker images
REPOSITORY                         TAG                 IMAGE ID            CREATED             SIZE
<my_dockerhub_login>/ui            2.0                 58d313016e6b        8 seconds ago       459MB
<my_dockerhub_login>/ui            1.0                 be26bf2af4d7        25 minutes ago      783MB
```
- Выключила созданные конты и запустила заново (с помощью тех же команд):
```sh
$ docker kill $(docker ps -q)
```
- Создала вольюм:
```sh
$ docker volume create reddit_db
```
- Пересоздала конты с подключением вольюма:
```sh
$ docker kill $(docker ps -q)
$ docker run -d --network=reddit --network-alias=post_db --network-alias=comment_db -v reddit_db:/data/db mongo:latest
$ docker run -d --network=reddit --network-alias=post <my_dockerhub_login>/post:1.0
$ docker run -d --network=reddit --network-alias=comment <my_dockerhub_login>/comment:1.0
$ docker run -d --network=reddit -p 9292:9292 <my_dockerhub_login>/ui:2.0
```
- Зашла на http://35.195.116.154:9292 создала новый пост
- Перпесоздала конты, проверила что пост остался на месте http://35.195.116.154:9292/post/5dd71a612e2264000e27ba04

- Стопнула и удалила все конты, остановила виртуалку
```sh
docker ps -qa | xargs docker stop
docker ps -qa | xargs docker rm
```

## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)

# HW 14. Docker: Network, docker-compose 

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/5

- Всё как обычно, подключилась к хосту:
```sh
$ docker-machine ls
$ eval $(docker-machine env docker-host)
# Просит пересоздать серт, тк стопала виртуалку
$ docker-machine regenerate-certs docker-host
$ eval $(docker-machine env docker-host)
```
### None network driver
- Запустила конт с none-драйвером. Образ joffotron/docker-net-tools с предустановелнными утилитами для работы с сетью (bind-tools, net-tools и curl).  
  Конт запустится, выполнит команду ifconfig и удалится.
```sh 
$ docker run -ti --rm --network none joffotron/docker-net-tools -c ifconfig
...
lo        Link encap:Local Loopback
          inet addr:127.0.0.1  Mask:255.0.0.0
          UP LOOPBACK RUNNING  MTU:65536  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000
          RX bytes:0 (0.0 B)  TX bytes:0 (0.0 B)
```
### Host network driver
- Запустила конт в сетевом пространстве docker-host.  
  На этот раз появились интерфейсы **br-1fbb4620178c Link encap, docker0, ens4, lo**
```sh
$ docker run -ti --rm --network host joffotron/docker-net-tools -c ifconfig
```
- Запустила то же самое с помощью docker-machine
```sh
$ docker-machine ssh docker-host ifconfig
```
- Запустила стопитсот раз (4) команду
```sh
$ docker run --network host -d nginx
$ docker ps -a
```
  Появилось 4 конта, каждый раз при запуске команды docker run стопался предыдущий конт (три находятся в состоянии Exited). nginx не может разворачиваться в одной и той же сети (без указания каких-либо параметров, типа порта) несколько раз, поэтому предыдущие стопаются.
- Остановила запущенный конт
```sh
$ docker kill $(docker ps -q)
```

### Docker networks
- Зашла на docker-host выполнила команду и посмотрела существующие в данный момент net-namespaces:
```sh
$ docker-machine ssh docker-host
$ sudo ln -s /var/run/docker/netns /var/run/netns
$ ip netns
```
- Запустила конт с использованием драйвера none, появился новый неймспейс, который не дает запустить в нем команду 
```sh
docker run --network none -d joffotron/docker-net-tools

ip netns
RTNETLINK answers: Invalid argument
RTNETLINK answers: Invalid argument
5643e4512ea8
default
```
- Запустила конт с драйвером host, неймспейс остался только дефолтный (тк совпадает с настройками, которые создаются при запуске с драйвером host), проверила какие интерфейсы в нем
```sh
docker run --network host -d nginx
ip netns
ip netns exec default ip a
```

### Bridge network driver
- Создала bridge-сеть в docker 
```sh
$ docker network create reddit --driver bridge
$ docker network ls
$ docker network inspect 1fbb4620178c
```
- Запустила проект reddit с использованием bridge-сети
```sh
$ docker run -d --network=reddit mongo:latest
$ docker run -d --network=reddit <my_login_dockerhub>/post:1.0
$ docker run -d --network=reddit <my_login_dockerhub>/comment:1.0
$ docker run -d --network=reddit -p 9292:9292 <my_login_dockerhub>/ui:1.0
```
Сервисы ссылаются друг на друга по dns-именам, прописанным в ENV-переменных (в Dockerfile).  
В нашем случае для решения проблемы, будем присваивать контам имена или сетевые алиасы при старте.  
```sh
--name <name> (можно задать только 1 имя)  
--network-alias <alias-name> (можно задать множество алиасов)
```
- Запуск новых контов
```sh
$ docker run -d --network=reddit --network-alias=post_db --network-alias=comment_db mongo:latest
$ docker run -d --network=reddit --network-alias=post <my_login_dockerhub>/post:1.0
$ docker run -d --network=reddit --network-alias=comment  <my_login_dockerhub>/comment:1.0
$ docker run -d --network=reddit -p 9292:9292 <my_login_dockerhub>/ui:1.0
```
- Проверка  
http://34.76.67.100:9292/new

- Запуск проекта в двух bridge сетях. Так, чтобы сервис ui не имел доступа к БД
  - Стопнула старые конты, создала docker-сети и запустила новые конты в разных бриджах
  ```sh
  $ docker kill $(docker ps -q) 

  $ docker network create back_net --subnet=10.0.2.0/24
  $ docker network create front_net --subnet=10.0.1.0/24
  $ docker network ls
  NETWORK ID          NAME                DRIVER              SCOPE
  029ff6b51819        back_net            bridge              local
  6636ac637c01        bridge              bridge              local
  7a368b0583c2        front_net           bridge              local
  1fbb4620178c        reddit              bridge              local

  $ docker run -d --network=front_net -p 9292:9292 --name ui  <my_login_dockerhub>/ui:1.0
  $ docker run -d --network=back_net --name comment  <my_login_dockerhub>/comment:1.0
  $ docker run -d --network=back_net --name post  <my_login_dockerhub>/post:1.0
  $ docker run -d --network=back_net --name mongo_db --network-alias=post_db --network-alias=comment_db mongo:latest
  ```
  - Docker при инициализации контейнера может подключить к нему только одну сеть. При этом контейнеры из соседних сетей не будут доступны как в DNS, так и для взаимодействия по сети. Поэтому нужно поместить контейнеры post и comment в обе сети.  
  Дополнительные сети подключаются командой:
  ```sh
  docker network connect <network> <container>
  ```
  - Подключила конты ко второй сети
  ```sh
  $ docker network connect front_net post
  $ docker network connect front_net comment
  ```
  - Проверка  
  http://34.76.67.100:9292/

### Команды
```sh
# Зашла на докер-хост и установила bridge-utils 
$ docker-machine ssh docker-host
docker-user@docker-host:~$ sudo apt-get update && sudo apt-get install bridge-utils

# Смотреть список сетей
$ sudo docker network ls

# Найти бриджи
$ ifconfig | grep br
br-029ff6b51819 Link encap:Ethernet  HWaddr 02:42:fb:5a:53:e1
br-1fbb4620178c Link encap:Ethernet  HWaddr 02:42:b3:07:d0:c2
br-7a368b0583c2 Link encap:Ethernet  HWaddr 02:42:7d:2e:a3:84

# Bridge для back_net (по аналогии и для остальных сетей)
$ ifconfig br-029ff6b51819
$ sudo docker inspect 029ff6b51819

# Смотреть инфу о bridge интерфейсе
$ sudo brctl show br-7a368b0583c2
## Отображаемые veth-интерфейсы - это те части виртуальных пар интерфейсов, которые лежат в сетевом пространстве хоста и также отображаются в ifconfig. Вторые их части лежат внутри контейнеров.

# Смотрим iptables
$ sudo iptables -nL -t nat
## Обратите внимание на цепочку POSTROUTING. Отмеченные звездочкой правила отвечают за выпуск во внешнюю сеть контейнеров из bridge-сетей
Chain POSTROUTING (policy ACCEPT)
target     prot opt source               destination
*MASQUERADE  all  --  10.0.2.0/24          0.0.0.0/0
*MASQUERADE  all  --  172.17.0.0/16        0.0.0.0/0
*MASQUERADE  all  --  172.18.0.0/16        0.0.0.0/0
MASQUERADE  tcp  --  10.0.1.2             10.0.1.2             tcp dpt:9292

## Обратите внимание на цепочку DOCKER и правила DNAT в ней. Они отвечают за перенаправление трафика на адреса уже конкретных контов
target     prot opt source               destination
DNAT       tcp  --  0.0.0.0/0            0.0.0.0/0            tcp dpt:9292 to:10.0.1.2:9292 

# Посмотреть процессы. Есть процесс docker-proxy, который слушает на порту 9292 
$ ps ax | grep docker-prox
20531 ?        Sl     0:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 9292 -container-ip 10.0.1.2 -container-port 9292
```

## Docker-compose
### Проблемы
- Одно приложение состоит из множества контейнеров/сервисов
- Один контейнер зависит от другого
- Порядок запуска имеет значение
- docker build/run/create ... (долго и много)

### Docker-compose
- Отдельная утилита
- Декларативное описание docker-инфраструктуры в YAML-формате
- Управление многоконтейнерными приложениями

**Установка [docker-compose](https://docs.docker.com/docker-for-mac/install/)**
```sh
$ docker-compose --version
docker-compose version 1.24.1, build 4667896b
```
- В дире src создала файл [docker-compose.yml](https://gist.githubusercontent.com/Lisskha/f1a9b76c0aa8ca2d8c748b53a994d224/raw/537d13118694276bf181ae3c5f2adc5538be0369/src%2520docker-compose.yml)
  - docker-compose поддерживает интерполяцию (подстановку) переменных окружения. В данном случае это переменная USERNAME. Поэтому перед запуском необходимо экспортировать значения данных переменных окружения.
- Остановила конты и выполнила их запуск с помощью компоса
```sh
$ docker kill $(docker ps -q)

$ export USERNAME=<my_login_dockerhub>
$ docker-compose up -d
$ docker-compose ps
$ docker ps
```
- Проверка  
http://34.76.67.100:9292/

## Задание 1
- Перед каждым пересозданием контов удаляю предыдущие
```sh
$ docker-compose down
```
- Для запуска контов
```sh
$ docker-compose up -d
```

- Добавила в [docker-compose.yml](https://gist.githubusercontent.com/Lisskha/f1a9b76c0aa8ca2d8c748b53a994d224/raw/8314f5a18901e1523608b28a9c2a7e6d21b91fda/src%2520docker-compose.yml%2520new) несколько сетей и параметризировала некоторые параметры. Параметризированные параметры добавила в src/.env (файл внесен в .gitignore), продублировала их в файл src/.env.example
- Результат
```sh
$ docker-compose ps
     Name                  Command             State           Ports
-----------------------------------------------------------------------------
src_comment_1   puma                          Up
src_post_1      python3 post_app.py           Up
src_post_db_1   docker-entrypoint.sh mongod   Up      27017/tcp
src_ui_1        puma                          Up      0.0.0.0:9292->9292/tcp
```
- Проверка  
http://34.76.67.100:9292/

## Задание 2
При запуске проекта с помощью docker-compose, все сущности создаются с префиксом = каталогу, где лежит docker-compose.yml. Это считается базовым именем проекта. Поменять его можно, закинув в .env параметр: **COMPOSE_PROJECT_NAME=<new_name>**

## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)

# HW 15. Gitlab CI: Построение процесса непрерывной поставки

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/6/files

- Необходимые параметры для машины, на которой будем разворачивать Gitlab CI
  ```sh
  1               CPU
  3.75GB          RAM 
  50-100GB        HDD 
  Ubuntu 16.04    IMAGE
  ```
  - В [официальной документации](https://docs.gitlab.com/ce/install/requirements.html) описаны рекомендуемые характеристики сервера 

- Создала новую ВМ с предустановленным докером
  ```sh
  $ docker-machine create --driver google \
  --google-machine-image https://www.googleapis.com/compute/v1/projects/ubuntu-os-cloud/global/images/family/ubuntu-1604-lts \
  --google-zone europe-west1-b \
  --google-machine-type n1-standard-1 \
  --google-disk-size 100 \
  gitlab-ci

  ...
  Docker is up and running!
  To see how to connect your Docker Client to the Docker Engine running on this virtual machine, run: 
  docker-machine env gitlab-ci
  ```
- Включила разрешение подключения по HTTP/HTTPS

Для запуска Gitlab CI мы будем использовать **omnibus-установку**  
Основной плюс для нас в том, что мы можем быстро запустить сервис и сконцентрироваться на процессе непрерывной поставки.  
Минусом такого типа установки является то, что такую инсталляцию тяжелее эксплуатировать и дорабатывать, но долговременная эксплуатация этого сервиса не входит в наши цели.
Более подробно об этом в документации  
https://docs.gitlab.com/omnibus/README.html  
https://docs.gitlab.com/omnibus/docker/README.html  

Установила докер сразу при создании ВМ, но можно было на пустую машину руками поставить:
```sh
# из-под root на новом сервере выполнить
# curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
# add-apt-repository "deb https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
# apt-get update
# apt-get install docker-ce docker-compose
```

### Подготовка окружения
- Зашла на ВМ, создала каталоги и подготовила [docker-compose.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/b782c399a746bc7017b97f86a0a21971bf66313e/srv%2520gitlab%2520docker-compose.yml)
  ```sh
  $ eval $(docker-machine env gitlab-ci)
  $ docker-machine ssh gitlab-ci
  
  sudo su
  mkdir -p /srv/gitlab/config /srv/gitlab/data /srv/gitlab/logs
  cd /srv/gitlab/
  vim docker-compose.yml
  ```
- Запустила сборку образа и запуск Gitlab CI (надо запускать в каталоге, где лежит docker-compose.yml)
  ```sh
  /srv/gitlab# docker-compose up -d
  ```
- Откуда взяли содержимое файла docker-compose.yml - https://docs.gitlab.com/omnibus/docker/README.html#install-gitlab-using-docker-compose  
- Проверка  
  http://34.76.67.100/users/password/edit?reset_password_token=psJktjUExEuCYk45-cyd
  Сменила пароль для рута, залогинилась.

## Работа с Gitlab CI
### Настройка
- Выкл регу новых юезров
  - В Settings/General/Sign-up restrictions сняла галку с Sign-up enabled 
### Создание проекта
***Из лекции:***
- Каждый проект в Gitlab CI принадлежит к группе проектов
- В проекте может быть определен CI/CD пайплайн
- Задачи (jobs), входящие в пайплайн, должны исполняться на runners 
 
***Создание группы***
- В Groups/Your Groups создать новую группу
- Заполнить описание 
 
***Создание проекта***
- Находясь в группе HW15, тыкнуть кнопку New project
- Имя проекта - example

***Добавление remote***
- В своей репе Lisskha_microservices в ветке gitlab-ci-1 запустить 
```sh
$ git remote add gitlab http://34.76.67.100/hw15/example.git
$ git push gitlab gitlab-ci-1
# Ввести креды, которые задавали в морде гитлаба
```

### CI/CD Pipeline
- Добавила файл [.gitlab-ci.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/a7fea23e38c25ecb2e0dfe8597d4ee7aa7534508/.gitlab-ci.yml) в корень своей репы
- Запушила в ветку
```sh
$ git add .
$ git commit -m 'Add pipeline definition'
$ git push gitlab gitlab-ci-1
```
- Если добавлять новый файл через морду, то не забыть потом спулить изменения 
```sh
git pull gitlab gitlab-ci-1
```
- Перейти в морде в CI / CD - Pipelines, там видно наш пайплайн. Но он пендится, тк нет раннера
- Запуск **Runner** и рега его в интерактивном режиме
  - Сначала надо получить токен. Идем в Settings/CI / CD/Runners settings - Expand
  - Копируем токен в разделе "Set up a specific Runner manually" 
  - На виртуалке с гитлабом запустить:
  ```sh
  docker run -d --name gitlab-runner --restart always \
  -v /srv/gitlab-runner/config:/etc/gitlab-runner \
  -v /var/run/docker.sock:/var/run/docker.sock \
  gitlab/gitlab-runner:latest
  ```
  - Runner запустился, регаемся
  ```sh
  docker exec -it gitlab-runner gitlab-runner register --run-untagged --locked=false

  Please enter the gitlab-ci coordinator URL (e.g. https://gitlab.com/):
  http://34.76.67.100/
  Please enter the gitlab-ci token for this runner:
  <token>
  Please enter the gitlab-ci description for this runner:
  [d8ee675a18ed]: runner-hw15
  Please enter the gitlab-ci tags for this runner (comma separated):
  linux,xenial,ubuntu,docker
  Registering runner... succeeded                     runner=tAaHjhDz
  Please enter the executor: parallels, shell, virtualbox, docker+machine, custom, docker, docker-ssh+machine, kubernetes, docker-ssh, ssh:
  docker
  Please enter the default Docker image (e.g. ruby:2.6):
  alpine:latest

  Runner registered successfully.
  ```
  - В настройках (в морде) появится новый раннер
  ```sh
  Runners activated for this project
  E3v_fsp6 
  runner-hw15
  docker linux ubuntu xenial
  ```
  - После добавления раннера, пайплайн запустился (в CI / CD/Pipelines)

### Тестирование reddit
- В свою репу качаем приложение, пушим в ветку в Gitlab
```sh
$ git clone https://github.com/express42/reddit.git && rm -rf ./reddit/.git
$ git add reddit/
$ git commit -m "Add reddit app"
$ git push gitlab gitlab-ci-1
```
- Изменила описание пайплайна в [.gitlab-ci.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/881dc945b0ffca094782031fc829848dc17935fe/.gitlab-ci.yml%2520new)
- В каталоге reddit создала файл [simpletest.rb](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/e66e10a873f2bc064a9f3d4d670deb38970dea15/reddit%2520simpletest.rb) для вызова тестов
- В reddit/Gemfile добавила библиотеку для тестирования
```sh
source 'https://rubygems.org'
...
gem 'rack-test'
...
end
```
- Теперь на каждое изменение в коде приложения будет запущен тест (смотреть в CI / CD - Jobs)

### Окружения
***DEV-окружение***

Вернемся к академическому пайплайну, который описывает шаги сборки, тестирования и деплоймента.  
В прошлом занятии мы создали job с названием deploy_job, но не разбирались что и куда будет задеплоено.  

Изменим пайплайн таким образом, чтобы job deploy стал определением окружения dev, на которое условно будет выкатываться каждое изменение в коде проекта.

Переименуем deploy stage в review.  
deploy_job заменим на deploy_dev_job  
Добавим environment  
Новый [.gitlab-ci.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/bdd355ab1c410c6abddb9d6584fee8dd40621aa1/.gitlab-ci.yml%2520new%25202) запушила в гитлаб
```sh
$ git add .gitlab-ci.yml
$ git commit -m "Update .gitlab-ci.yml for DEV"
$ git push gitlab gitlab-ci-1
```

После успешного завешения пайплайна с определением окружения перейти в Operations > Environments, там появилось определение первого окружения (dev)  

***PROD-окружение и STAGE-окружение***  

Если на dev мы можем выкатывать последнюю версию кода, то к production окружению это может быть неприменимо, если, конечно, вы не стремитесь к continuous deployment.  
Определим два новых этапа: stage и production, первый будет содержать job имитирующий выкатку на staging окружение, второй на production окружение.
Определим эти job таким образом, чтобы они запускались с кнопки  
Новый файл [.gitlab-ci.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/d89b7b2c68dd3ee9cb7ef143d0ae6da4c77316a3/.gitlab-ci.yml%2520new%25203%2520STAGE%2520and%2520PROD) запушила в гитлаб
```sh
$ git add .gitlab-ci.yml
$ git commit -m "Update .gitlab-ci.yml for STAGE & PROD"
$ git push gitlab gitlab-ci-1
```
when: manual – говорит о том, что job должен быть запущен человеком из UI.  

Теперь в пайплайне стейдж и прод не запустились автоматом, их нужно запускать вручную.  
На странице окружений в Operations > Environments появились оружения staging и production  

Обычно, на production окружение выводится приложение с явно зафиксированной версией (например, 2.4.10).  
Добавим в описание pipeline директиву, которая не позволит нам выкатить на staging и production код, не помеченный с помощью тэга в git.  
```sh
# В staging и production перед script нужно добавить 
only:
- /^\d+\.\d+\.\d+/
```
Директива only описывает список условий, которые должны быть истинны, чтобы job мог запуститься.  
Регулярное выражение слева означает, что должен стоять semver тэг в git, например, 2.4.10  

Изменение без указания тэга запустят пайплайн без job staging и production  
Изменение, помеченное тэгом в git запустит полный пайплайн
```sh
$ git add .gitlab-ci.yml
$ git commit -m "Update .gitlab-ci.yml Add tag"
$ git tag 2.4.10
$ git push gitlab gitlab-ci-1 --tags
```

***Динамические окружения***  
Gitlab CI позволяет определить динамические окружения, это мощная функциональность позволяет вам иметь выделенный стенд для, например, каждой feature-ветки в git.  
Определяются динамические окружения с помощью переменных, доступных в .gitlab-ci.yml  
Новый файл [.gitlab-ci.yml](https://gist.githubusercontent.com/Lisskha/a26e4c3f6ff7d94656fd1eb6a624131b/raw/6294510fa2da3ec53d90acce677703a40a83393a/.gitlab-ci.yml%2520new%25204%2520Dynamic%2520environment), где only и except в этом job, определяют динамическое окружение для каждой ветки в репозитории, кроме ветки master  

Теперь, на каждую ветку в git отличную от master Gitlab CI будет определять новое окружение.
Если создать ветки new-feature и bugfix, то на странице окружений они будут в review

## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)

# HW 16. Введение в мониторинг

PR:  

## Подготовка окружения
- Создала правила фаервола для Prometheus и Puma
  ```sh
  $ gcloud compute firewall-rules create prometheus-default --allow tcp:9090
  $ gcloud compute firewall-rules create puma-default --allow tcp:9292
  ```
- Создала Docker хост в GCE и настроила локальное окружение на работу с ним
  ```sh
  $ export GOOGLE_PROJECT=docker-xxxxxx
  $ docker-machine create --driver google --google-machine-image https://www.googleapis.com/compute/v1/projects/ubuntu-os-cloud/global/images/family/ubuntu-1604-lts --google-machine-type n1-standard-1 --google-zone europe-west1-b docker-host
  ...
  Docker is up and running!

  $ eval $(docker-machine env docker-host)
  ```
- Когда меняется IP для докер-хоста, надо перегенерить серт
  ```sh
  $ docker-machine regenerate-certs docker-host
  $ eval $(docker-machine env docker-host) 
  ```

## Запуск Prometheus и описание web-интерфейса

- Систему мониторинга Prometheus будем запускать внутри Docker контейнера. Взяли образ с DockerHub
  ```sh
  $ docker run --rm -p 9090:9090 -d --name prometheus prom/prometheus:v2.1.0
  ```
- Прометей доступен по адресу  
  http://35.195.16.1:9090/  
  По умолчанию сервер слушает на порту 9090, а IP адрес созданной VM можно узнать, используя команду:
  ```sh
  $ docker-machine ip docker-host 
  ```

### Интерфейс
- Строка ввода выражений для получения и анализа информации мониторинга (метрик) из хранилища
- Выполнение запроса - кнопка **Execute**
- Выбор имеющихся метрик
- Вкладка **Console** - выводит численное значение выражений
- Вкладка **Graph** - строит график изменений значений метрик со временем
- Клик по **"insert metric at cursor"** - Prometheus уже собирает какие-то метрики. По дефолту он собирает статистику о своей работе. Выбрала метрику *prometheus_build_info* - можно увидеть информацию о версии
  ```sh
  prometheus_build_info{branch="HEAD",goversion="go1.9.2",instance="localhost:9090",job="prometheus",revision="85f23d82a045d103ea7f3c89a91fba4a93e6367a",version="2.1.0"}	1
  ```
  - **prometheus_build_info** - это ***название метрики*** - идентификатор собранной информации
  - **branch,goversion,instance,job,revision,version** - это ***лейблы*** - добавляют метаданных метрике, уточняют ее. Использование лейблов дает нам возможность не ограничиваться лишь одним названием метрик для идентификации получаемой информации. Лейблы содержаться в {} скобках и представлены наборами **"ключ=значение"**
  - **1** - это ***значение метрики*** - численное значение метрики, либо NaN, если значение недоступно
- **Targets** (Status/Targets) - системы или процессы, за которыми следит Prometheus. Prometheus является pull системой, поэтому он постоянно делает HTTP запросы на имеющиеся у него адреса (***endpoints***). Текущий список целей
  ```sh
  prometheus (1/1 up)

  Endpoint	              State  Labels	                Last Scrape	  Error
  http://localhost:9090/metrics UP     instance="localhost:9090"  5.873s ago	
  ```
  - В Targets сейчас только сам Prometheus. У каждой цели есть свой список адресов (endpoints), по которым следует обращаться для получения информации
  - В веб интерфейсе можно увидеть 
    - **состояние endpoint-а** (up); 
    - **лейбл** (instance="someURL"), который Prometheus автоматически добавляет к каждой метрике, получаемой с данного endpoint-а;
    - **время** (Last Scrape), прошедшее с момента последней операции сбора информации с endpoint-а;
    - **ошибки** (Error) отображаются при их наличии и можно отфильтровать только неживые таргеты
  - Можно открыть страницу в браузере по указанному HTTP пути (host:port/metrics), чтобы посмотреть, как выглядит та информация, которую собирает Prometheus  
  http://35.195.16.1:9090/metrics
  
## Создание Docker образа и конфиг прометея

- Стопнула созданный конт
  ```sh
  $ docker stop prometheus
  ```
- Переупорядочила структуру директорий
  - Создала диру docker, перенесла в нее docker-monolith, .env*, docker-compose.*
  - Создала диру monitoring
- С этого момента сборка сервисов отделена от docker-compose, поэтому инструкции build можно удалить из [docker-compose.yml](https://gist.githubusercontent.com/Lisskha/af4af07c942ec73edc5d9a9ff7115fbe/raw/c3bd1e587fa4ae25e9307691b1dc5eaee5da7df4/docker%2520docker-compose.yml)
### !!! Не забывать править .gitignore !!!
- Соберем на основе готового образа с DockerHub свой Docker образ с конфигурацией для мониторинга микросервисов.  
  Создала диру monitoring/prometheus и файл monitoring/prometheus/Dockerfile:
  ```sh
  FROM prom/prometheus:v2.1.0
  ADD prometheus.yml /etc/prometheus/
  ```
- Вся конфигурация Prometheus происходит через файлы конфигурации и опции командной строки. Создала конф файл для сбора метрик с микросервисов - [monitoring/prometheus/prometheus.yml](https://gist.githubusercontent.com/Lisskha/af4af07c942ec73edc5d9a9ff7115fbe/raw/c3bd1e587fa4ae25e9307691b1dc5eaee5da7df4/monitoring%2520prometheus%2520prometheus.yml)
- В директории prometheus собираем Docker образ
  ```sh
  $ export USER_NAME=<my_dockerhub_login>
  $ docker build -t $USER_NAME/prometheus .
  ```
- В коде микросервисов есть healthcheck-и для проверки работоспособности приложения. Сборку образов теперь необходимо производить при помощи скриптов docker_build.sh, которые есть в директории каждого сервиса. С его помощью мы добавим информацию из Git в наш healthcheck.  
Запустить из корня репы сборку образов:
  ```sh
  $ for i in ui post-py comment; do cd src/$i; bash docker_build.sh; cd -; done
  ```
- Поднимаем прометей совместно с микросервисами. В файл **docker/docker-compose.yml** добавила новый сервис `prometheus`, заменила директивы build на image. Итоговый файл - [gist](https://gist.githubusercontent.com/Lisskha/af4af07c942ec73edc5d9a9ff7115fbe/raw/6f88b2ffac43346855b92799b378367885e1d5e6/docker%2520docker-compose.yml%2520new)
- Будем юзать Prometheus для мониторинга всех микросервисов, поэтому необходимо, чтобы контейнер с ним мог общаться по сети со всеми другими сервисами.  
  - Добавила в определение сервиса prometheus в компоуз файле секцию networks
  - Подправила .env и .env.example
- Подняла сервисы, определенные в docker/docker- compose.yml (находясь в каталоге с композ-файлом)
  ```sh
  $ docker-compose up -d
  ```
- Проверка, что запустилось приложение и прометей  
http://35.195.16.1:9292/  
http://35.195.16.1:9090/graph

## Мониторинг состояния микросервисов
- Проверить список endpoint-ов, с которых собирает информацию Prometheus, и убедиться, что они в состоянии UP можно в таргетах - Status/Targets
  ```sh
  comment (1/1 up) 
  Endpoint	             State	
  http://comment:9292/metrics  UP	

  prometheus (1/1 up) 
  Endpoint	              State	
  http://localhost:9090/metrics UP

  ui (1/1 up) 
  Endpoint	              State	
  http://ui:9292/metrics        UP
  ```
- **Healthcheck-и** представляют собой проверки того, что сервис здоров и работает в ожидаемом режиме. В нашем случае healthcheck выполняется внутри кода микросервиса и выполняет проверку того, что все сервисы, от которых он зависит, ему доступны.  
  Если требуемые для его работы сервисы здоровы, то healthcheck проверка возвращает **status = 1**  
  Если один из нужных ему сервисов нездоров или недоступен, то проверка вернет **status = 0**
  - В морде прометея выполнила поиск по метрике ***ui_health***  
  Во вкладке Console помимо имени метрики и ее значения, видно информацию о версии приложения, коммите и ветке кода в Git
  ```sh
  ui_health{branch="monitoring-1",commit_hash="4d6c71f",instance="ui:9292",job="ui",version="0.0.1"}	1
  ``` 
- Сервис считается здоровым, если все сервисы, от которых он зависит также являются здоровыми. Если остановить сервис post, то статус ui сервиса изменится на 0 (видно на графике и во вкладке консоль в поле Value)
  ```sh
  $ docker-compose stop post
  ```
  - Поиск проблемы - в строке выражений можно набрать ***ui_health_*** и увидеть название метрик сервисов, от которых зависит сервис ui.  
  Смотрим состояние метрик ***ui_health_comment_availability*** (Value=1) и ***ui_health_post_availability*** (Value=0)  
  Чиним сервис post:
    ```sh
    $ docker-compose start post
    ```

## Exporters

- **Экспортер** похож на вспомогательного агента для сбора метрик.  
  `В ситуациях, когда мы не можем реализовать отдачу метрик Prometheus в коде приложения, можно использовать экспортер, который будет транслировать метрики приложения или системы в формате доступном для чтения Prometheus`
  - Программа, которая делает метрики доступными для сбора Prometheus
  - Дает возможность конвертировать метрики в нужный для Prometheus формат
  - Используется когда нельзя поменять код приложения
  - Примеры: PostgreSQL, RabbitMQ, Nginx, Node exporter, cAdvisor

### Node exporter
Для сбора инфы о работе Докер-хоста и предоставления этой инфы в прометей, будем использовать [Node exporter](https://github.com/prometheus/node_exporter)  
- Node экспортер будет запускаться также в контейнере. В [docker/docker-compose.yml]() определила сервис `node-exporter`, добавила определение сетей для этого сервиса, чтобы прометей мог достучаться до экспортера.
- Чтобы сказать Prometheus следить за еще одним сервисом, нужно добавить информацию о нем в конфиг [monitoring/prometheus/prometheus.yml](https://gist.githubusercontent.com/Lisskha/af4af07c942ec73edc5d9a9ff7115fbe/raw/1fbaf126bdd4f4c221605f47e3aef193b788a213/monitoring%2520prometheus%2520prometheus.yml%2520new) (добавить еще job) в раздел *scrape_configs* 
  ```sh
  - job_name: 'node'
    static_configs:
      - targets:
        - 'node-exporter:9100'
  ```
- Собрала новый образ для Prometheus (находясь в каталоге monitoring/prometheus/)
  ```
  $ docker build -t $USER_NAME/prometheus .
  ```
- Перешла в каталог docker/ (где находится композ файл), пересоздала конты с сервисами
  ```sh
  $ docker-compose down && docker-compose up -d
  ```
- В прометее появился еще один endpoint
  ```
  node (1/1 up) 
  Endpoint	                  State	Labels	                       Last Scrape	Error
  http://node-exporter:9100/metrics UP	instance="node-exporter:9100"	3.278s ago	
  ```
- Теперь можно посмотреть инфу и график, например, об LA - метрика *node_load1*

### Проверка работы мониторинга
- Зашла на хост
  ```
  $ docker-machine ssh docker-host
  ```
- Добавила нагрузку и проверила график в прометее
  ```
  $ yes > /dev/null
  ```
  http://35.195.16.1:9090/graph?g0.range_input=1h&g0.expr=node_load1&g0.tab=0

### Запушить образы в DockerHub
- `$ docker login`
- `$ docker push $USER_NAME/ui`
- `$ docker push $USER_NAME/comment`
- `$ docker push $USER_NAME/post`
- `$ docker push $USER_NAME/prometheus`
- Мой репозиторий https://hub.docker.com/u/yulka

- Удалить виртуалку
  ```
  $ docker-machine rm docker-host
  ```

## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)