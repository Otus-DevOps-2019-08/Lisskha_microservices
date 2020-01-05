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
- [HW16. Введение в мониторинг](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-16-%D0%B2%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B2-%D0%BC%D0%BE%D0%BD%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%BD%D0%B3)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-4)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-4)
- [HW17. Мониторинг приложения и инфраструктуры](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-17-%D0%BC%D0%BE%D0%BD%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%BD%D0%B3-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F-%D0%B8-%D0%B8%D0%BD%D1%84%D1%80%D0%B0%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D1%8B)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-5)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-5)
- [HW18. Логирование и распределенная трассировка](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#hw-18-%D0%BB%D0%BE%D0%B3%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B8-%D1%80%D0%B0%D1%81%D0%BF%D1%80%D0%B5%D0%B4%D0%B5%D0%BB%D0%B5%D0%BD%D0%BD%D0%B0%D1%8F-%D1%82%D1%80%D0%B0%D1%81%D1%81%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D0%B0)
    - [Доп. задание №1](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-1-6)
    - [Доп. задание №2](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#%D0%B4%D0%BE%D0%BF-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-2-6)
- [HW19. Введение в Kubernetes]()
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

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/11/files

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
- Node экспортер будет запускаться также в контейнере. В [docker/docker-compose.yml](https://gist.githubusercontent.com/Lisskha/af4af07c942ec73edc5d9a9ff7115fbe/raw/1fbaf126bdd4f4c221605f47e3aef193b788a213/docker%2520docker-compose.yml%2520new%25202) определила сервис `node-exporter`, добавила определение сетей для этого сервиса, чтобы прометей мог достучаться до экспортера.
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


# HW 17. Мониторинг приложения и инфраструктуры

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/14/files

## Подготовка окружения

`!!! Открывать порты в файрволле для новых сервисов нужно самостоятельно по мере их добавления !!!`

- Создала Docker хост в GCE и настроила локальное окружение на работу с ним
  ```
  $ export GOOGLE_PROJECT=docker-xxxxxx
  $ docker-machine create --driver google \
     --google-machine-image https://www.googleapis.com/compute/v1/projects/ubuntu-os-cloud/global/images/family/ubuntu-1604-lts \
     --google-machine-type n1-standard-1 \
     --google-zone europe-west1-b \
     docker-host-2
  $ eval $(docker-machine env docker-host-2)
  $ docker-machine ip docker-host-2
  35.241.234.193
  ```
- Разделила файлы Docker Compose:
  - Описание приложений оставила в [docker-compose.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/c0c61ba29f344577311dcbd0f9a7b5b0cc5a5212/docker%2520docker-compose.yml)
  - Мониторинг вынесла в файл [docker-compose-monitoring.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/c0c61ba29f344577311dcbd0f9a7b5b0cc5a5212/docker%2520docker-compose-monitoring.yml)
  - Теперь для запуска приложений:
    ```
    docker-compose up -d
    ```
  - А для мониторинга:
    ```
    docker-compose -f docker-compose-monitoring.yml up -d
    ```

## cAdvisor

Мы будем использовать [cAdvisor](https://github.com/google/cadvisor) для наблюдения за состоянием Docker контейнеров.  
**cAdvisor** собирает информацию о ресурсах, потребляемых контейнерами и характеристиках их работы. Например: % использования контом проца и памяти, объем сетевого трафа и тд.  

- cAdvisor также будет запускаться в контейнере. Для этого добавила новый сервис в файл [docker- compose-monitoring.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/c898a1363ec5e306a7e014d7f6f2de1a99e68d10/docker%2520docker-compose-monitoring.yml%2520new1) и определила настройки сети для сервиса `cadvisor`, чтобы прометей мог собирать с него метики
  ```sh
    cadvisor:
    image: google/cadvisor:v0.29.0
    volumes:
      - '/:/rootfs:ro'
      - '/var/run:/var/run:rw'
      - '/sys:/sys:ro'
      - '/var/lib/docker/:/var/lib/docker:ro'
    ports:
      - '8080:8080'
    networks:
      - front_net
      - back_net
  ```  
- Открыла порт 8080 в GCE
  ```
  $ gcloud compute firewall-rules list
  $ gcloud compute firewall-rules create cadvisor-default --allow tcp:8080
  ```
- Добавила информацию о новом сервисе в конфигурацию Prometheus в файл [monitoring/prometheus/prometheus.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/dde5fa7045e27df1de97983502e65beed44656b8/monitoring%2520prometheus%2520prometheus.yml)
  ```
  - job_name: 'cadvisor'
    static_configs:
      - targets:
        - 'cadvisor:8080'
  ```
- И пересобрала образ Prometheus (находясь в каталоге monitoring/prometheus/)
  ```sh
  $ export USER_NAME=<my_dockerhub_login>
  $ docker build -t $USER_NAME/prometheus .
  ```
- Запустила сервисы
  ```sh
  # Запустила создание образов, находясь в корне репы
  $ for i in ui post-py comment; do cd src/$i; bash docker_build.sh; cd -; done

  # Запустила создание сервисов, находясь в каталоге docker/
  $ docker-compose up -d 
  $ docker-compose -f docker-compose-monitoring.yml up -d
  ```
- Проверка  
  - Приложение  
  http://35.241.234.193:9292/
  - Prometheus  
  http://35.241.234.193:9090/graph
  - cAdvisor  
  http://35.241.234.193:8080/containers/

### cAdvisor UI
`cAdvisor имеет UI, в котором отображается собираемая о контейнерах информация`, он доступен по адресу http://35.241.234.193:8080 
- **[Docker Containers](http://35.241.234.193:8080/docker/)** - просмотр информации по контейнерам
  - `Subcontainers` - список контейнеров, запущенных на хосте
  - `Driver Status` - информацию о хосте
  - `Images` - информацию об образах контейнеров 
- Если [нажать](http://35.241.234.193:8080/docker/e33ef828cc27b2ea3802dbd02e40479e5f39af36f2284f50525e9de329800e81) на один из контов, то можно посмотреть информацию о его работе
  - Здесь отображается информация по процессам, использованию CPU, памяти, сети и файловой системы
- По пути `/metrics` все собираемые метрики публикуются для сбора Prometheus  
  http://35.241.234.193:8080/metrics
  - имена метрик контейнеров начинаются со слова `container`
- Проверим, что метрики контейнеров собираются **Prometheus**. В морде прометея http://35.241.234.193:9090/graph ввела слово `container` - появилось много вариантов дополнения имени метрики. Для примера посмотрела метрику `container_cpu_system_seconds_total` - в консоли и на графике корректно отобразились данные.

## Визуализация метрик: Grafana

`Будем использовать инструмент Grafana для визуализации данных из Prometheus`
- Добавила сервис `grafana` в [docker-compose-monitoring.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/46a1fefa628de5b9988fc0909c75591d16a6f146/docker%2520docker-compose-monitoring.yml%2520new2) и определила настройки сети для сервиса
  ```sh
    grafana:
      image: grafana/grafana:5.0.0
      volumes:
        - grafana_data:/var/lib/grafana
      environment:
        - GF_SECURITY_ADMIN_USER=admin
        - GF_SECURITY_ADMIN_PASSWORD=secret
      depends_on:
        - prometheus
      ports:
        - '3000:3000'
      networks:
        - front_net
        - back_net
  volumes:
    prometheus_data:
    grafana_data: 
  ```
- Открыла порт 3000 в GCE
  ```
  $ gcloud compute firewall-rules create grafana-default --allow tcp:3000
  ```
- Запуск сервиса grafana
  ```
  $ docker-compose -f docker-compose-monitoring.yml up -d grafana
  ```

### Grafana UI

Доступна по адресу http://35.241.234.193:3000/login  
Креды те, что передавали через переменные окружения.
- Добавление источника данных
  - Add data source
  - Name: Prometheus Server 
  - Type: Prometheus
  - URL: http://prometheus:9090 
  - Access: Proxy
  - И затем нажмем Add
- Дашборды
  - На [сайте Grafana](https://grafana.com/grafana/dashboards) есть готовые даши, которые можно скачать
  - Выберем в качестве источника данных - Prometheus, категорию - Docker. И выбираем популярный даш [Docker and system monitoring](https://grafana.com/grafana/dashboards/893)
  - Скачала json ***Download JSON***. В дире monitoring создала директории `mkdir -p grafana/dashboards`, куда перенесла скачанный файл и переименовала его в DockerMonitoring.json
  - Импорт дашборда - в морде Create/Import --> Upload .json --> path-to-DockerMonitoring.json
    - **Name** Docker and system monitoring
    - **Prometheus** Prometheus Server
    - **Import**
  - Появился даш с графиками с информацией о состоянии хостовой системы и работе контейнеров

## Мониторинг работы приложения

- В качестве примера метрик приложения в **сервис UI** [были добавлены](https://github.com/express42/reddit/commit/e443f6ab4dcf25f343f2a50c01916d750fc2d096):
  - `счетчик ui_request_count`, который считает каждый приходящий HTTP-запрос (добавляя через лейблы такую информацию как HTTP метод, путь, код возврата, мы уточняем данную метрику) 
  - `гистограмма ui_request_latency_seconds`, которая позволяет отслеживать информацию о времени обработки каждого запроса
- В качестве примера метрик приложения в **сервис Post** [была добавлена](https://github.com/express42/reddit/commit/d8a0316c36723abcfde367527bad182a8e5d9cf2):
  - `гистограмма post_read_db_seconds`, которая позволяет отследить информацию о времени требуемом для поиска поста в БД
- Добавила информацию о post-сервисе в конфигурацию Prometheus [monitoring/prometheus/prometheus.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/20cbbbd538c01bcaded381703d7503add646d9d1/monitoring%2520prometheus%2520prometheus.yml%2520new1), чтобы он начал собирать метрики и с него:
  ```sh
    - job_name: 'post'
    static_configs:
      - targets:
        - 'post:5000'
  ```
- Пересобрала образ Prometheus
  ```sh
  $ export USER_NAME=<my_dockerhub_login>
  $ docker build -t $USER_NAME/prometheus .
  ``` 
- Добавила порт 5000 в GCE
  ```sh
  $ gcloud compute firewall-rules create post-default --allow tcp:5000
  ```
- Пересоздала Docker инфраструктуру мониторинга
  ```
  $ docker-compose -f docker-compose-monitoring.yml down
  $ docker-compose -f docker-compose-monitoring.yml up -d
  ```
- В морде приложения добавила несколько постов и комментов, чтобы собрать значения метрик приложения

### Dashboard

- Создала даш в графане Create/Dashboard
  - "Построить график" **New Panel --> Graph**
  - **Panel Title --> Edit**
  - График изменения счетчика HTTP-запросов по времени
    - **Data Source:** Prometheus Server
    - **A:** ui_request_count
  - Изменить заголовок графика и описание можно во вкладке  `General`
    - **Title:** UI HTTP requests
    - **Description:** All HTTP requests that UI service receives
  - Добавила еще один график для запросов, которые будут возвращать код ошибки 
    - **Add Panel --> Graph / Edit**
    - В поле запросов запишем выражение для поиска всех http запросов, у которых код возврата начинается либо с 4 либо с 5. Для этого используется функция `rate()`, чтобы посмотреть не просто значение счетчика за весь период наблюдения, но и скорость увеличения данной величины за промежуток времени (возьмем, к примеру 1- минутный интервал, чтобы график был хорошо видим)
      ```
      rate(ui_request_count{http_status=~"^[45].*"}[1m])
      ```
    - График ничего не покажет, если не было запросов с ошибочным кодом возврата. Для проверки можно перейти по несуществующему пути http://35.241.234.193:9292/nonexistent, чтобы получить 404. На графике появится метрика ошибки
  - Смотреть хистори изменений борды - **Settings/Versions**
  - Применила функцию rate() для первого графика
    ```
    rate(ui_request_count{http_status=~"^[23].*"}[1m])
    ```

### Гистограмма

***Гистограмма*** представляет собой графический способ представления распределения вероятностей некоторой случайной величины на заданном промежутке значений. Для построения гистограммы берется *интервал значений*, который может принимать измеряемая величина и разбивается на промежутки (обычно одинаковой величины), данные промежутки помечаются *на горизонтальной оси X*. Затем над каждым интервалом рисуется прямоугольник, высота которого соответствует числу измерений величины, попадающих в данный интервал.  
Простым **примером гистограммы** может быть распределение оценок за контрольную в классе, где учится 21 ученик. Берем промежуток возможных значений (от 1 до 5) и разбиваем на равные интервалы. Затем на каждом интервале рисуем столбец, высота которого соответсвует частоте появлению данной оценки.  
В Prometheus есть тип метрик `histogram`. Данный тип метрик в качестве своего значение *отдает ряд распределения измеряемой величины в заданном интервале значений*. Мы используем данный тип метрики *для измерения времени обработки HTTP запроса нашим приложением*.  

- Рассмотрим пример гистограммы в Prometheus. Посмотрим информацию по времени обработки запроса приходящих на главную страницу приложения
  ```
  ui_request_response_time_bucket{path="/"}
  ```
- Полученные значения означают, что запросов с временем обработки <= 0.025s было 8 штук, запросов <= 0.05s было 21шт (в этот столбец входят 8 запросов из предыдущего столбца и 13 запросов из промежутка [0.025s; 0.05s], такую гистограмму еще называют **кумулятивной**), запросов <=0.1 было 22шт. Запросов, которые бы заняли > 0.1s на обработку не было, поэтому величина всех последующих столбцов равна 22

### Процентиль

- Числовое значение в наборе значений
- Все числа в наборе меньше процентиля, попадают в границы заданного процента значений от всего числа значений в наборе
- **Пример**  
  В классе 20 учеников. Ваня занимает 4-е место по росту в классе. Тогда рост Вани (180 см) является 80-м процентилем. Это означает, что 80 % учеников имеют рост менее 180 см.
- **95-й процентиль**   
  Часто для анализа данных мониторинга применяются значения `90, 95 или 99-й процентиля`  
  Мы вычислим 95-й процентиль для выборки времени обработки запросов, чтобы посмотреть какое значение является максимальной границей для большинства (95%) запросов. Для этого воспользуемся встроенной функцией `histogram_quantile()`
  ```
  histogram_quantile(0.95, sum(rate(ui_request_response_time_bucket[5m])) by (le))
  ```

Итоговый дашборд экспортнула в файл UI_Service_Monitoring.json, положила его в monitoring/grafana/dashboards  

### Сбор метрик бизнес-логики

- В качестве примера метрик бизнес логики в приложение были добавлены счетчики количества постов и комментариев
  - post_count
  - comment_count
- Построим график скорости роста значения счетчика за последний час, используя функцию rate()
  - Создала даш Business_Logic_Monitoring
  - Создала график с функцией rate() для подсчета постов 
    ```
    rate(post_count[1h])
    ```
  - Подолбный график для подсчета комментов
    ```
    rate(comment_count[1h])
    ```
- Новый дашборд экспортнула в файл monitoring/grafana/dashboards/Business_Logic_Monitoring.json

## Алертинг

### Правила алертинга
Определим несколько правил, в которых зададим условия состояний наблюдаемых систем, при которых мы должны получать оповещения, т.к. заданные условия могут привести к недоступности или неправильной работе нашего приложения.  
**P.S.** В самой Grafana тоже есть alerting. Но по функционалу он уступает Alertmanager в Prometheus.

### Alertmanager
**`Alertmanager`** - дополнительный компонент для системы мониторинга Prometheus, который отвечает за первичную обработку алертов и дальнейшую отправку оповещений по заданному назначению.  
Создала диру monitoring/alertmanager/ и Dockerfile в ней, с содержимым:
```sh
FROM prom/alertmanager:v0.14.0
ADD config.yml /etc/alertmanager/
``` 
Настройки Alertmanager-а задаются через YAML файл или опции командой строки.  
- В слаке (DevOps team) созала свой Incoming Webhook
- Создала файл [monitoring/alertmanager/config.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/7628c423e5ed2041cb5a150298869d2175f9f5fc/monitoring%2520alertmanager%2520config.yml) для отправки нотификаций в тестовый слак канал yuliya_kharchenko
- Собрала образ alertmanager (находясь в каталоге monitoring/alertmanager/) 
  ```
  $ export USER_NAME=<my_dockerhub_login>
  $ docker build -t $USER_NAME/alertmanager .
  ```
- Добавила сервис alertmanager в файл [docker/docker-compose-monitoring.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/ed3ac0eb435be9cd20a715cde0092b463c102c2f/docker%2520docker-compose-monitoring.yml%2520new3), сервис добавила в одну сеть с прометеем
  ```
  alertmanager:
    image: ${USERNAME}/alertmanager
    command:
      - '--config.file=/etc/alertmanager/config.yml'
    ports:
      - '9093:9093'
    networks:
      - front_net
      - back_net 
  ```
- Добавила порт 9093 в GCE
  ```
  $ gcloud compute firewall-rules create alertmanager-default --allow tcp:9093
  ```
- Создала файл [monitoring/prometheus/alerts.yml](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/850f22bb421bbba5b2fe91ccfb0291940fb6df2b/monitoring%2520prometheus%2520alerts.yml) для определения условий срабатывания алертов и отправки их алертманагеру.  
  - Создала алерт, который будет срабатывать, когда один из endpoint'ов недоступен (метрика `up` будет равна нулю)  
  - Добавила операцию копирования данного файла в Dockerfile monitoring/prometheus/Dockerfile
    ```
    ...
    ADD alerts.yml /etc/prometheus/
    ```
- Добавила инфу о правилах в [конфиг прометея](https://gist.githubusercontent.com/Lisskha/86501949f5fbbf798592b94f82caec62/raw/57bc1d1debbc0012ef515dec80c373ab440954ec/monitoring%2520prometheus%2520prometheus.yml%2520new2)
- Пересобрала образ прометея
  ```
  $ docker build -t $USER_NAME/prometheus .
  ```
- Пересоздала инфраструктуру мониторинга
  ```
  $ docker-compose -f docker-compose-monitoring.yml down
  $ docker-compose -f docker-compose-monitoring.yml up -d
  ```
- Для проверки стопнула один сервис `$ docker-compose stop post`, в канал слака прилетел алерт 
  ```
  AlertManagerAPP
  [FIRING:1] InstanceDown (post:5000 post page)
  ```
- Морда алертманагера доступна по адресу  
  http://35.241.234.193:9093

### Запушить образы в DockerHub
- `$ docker login`
- `$ docker push $USER_NAME/ui`
- `$ docker push $USER_NAME/comment`
- `$ docker push $USER_NAME/post`
- `$ docker push $USER_NAME/prometheus`
- Мой репозиторий https://hub.docker.com/u/yulka

- Удалить виртуалку
  ```
  $ docker-machine rm docker-host-2
  ```

## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)


# HW 18. Логирование и распределенная трассировка

PR: https://github.com/Otus-DevOps-2019-08/Lisskha_microservices/pull/18/files 

## Подготовка окружения
- Код микросервисов обновился для добавления функционала логирования. Клонировала новую версию кода по [ссылке](https://github.com/express42/reddit/tree/logging) и обновила код в дире /src
- Если вы используется python-alpine, добавьте в /src/post-py/Dockerfile установку пакетов gcc и musl-dev
  ```
  ...

  RUN apk add --no-cache --virtual .build-deps gcc musl-dev \
    && pip install --no-cache-dir -r $APP_HOME/requirements.txt \
    && apk del .build-deps

  ...
  ```
### !!! Открывать порты в файрволле для новых сервисов нужно самостоятельно по мере их добавления !!!
- Создала Docker хост в GCE и настроила локальное окружение на работу с ним
  ```
  $ export GOOGLE_PROJECT=docker-xxxxxx

  $ docker-machine create --driver google --google-machine-image https://www.googleapis.com/compute/v1/projects/ubuntu-os-cloud/global/images/family/ubuntu-1604-lts --google-machine-type n1-standard-1 --google-open-port 5601/tcp --google-open-port 9292/tcp --google-open-port 9411/tcp logging
  
  $ eval $(docker-machine env logging)

  $ docker-machine ip logging
  108.59.80.183

  $ gcloud compute firewall-rules list
  docker-machines         default  INGRESS    1000      tcp:2376,tcp:5601,tcp:9292,tcp:9411        False
  ```
- Выполнила сборку образов из корня репы
  ```
  $ export USER_NAME=yulka

  $ for i in ui post-py comment; do cd src/$i; bash docker_build.sh; cd -; done
  ```
### !!! Внимание! В данном ДЗ мы используем отдельные теги для контейнеров приложений :logging !!!

## Логирование Docker контейнеров
### Elastic Stack

Как упоминалось на лекции хранить все логи стоит **централизованно**: на одном/нескольких серверах. В этом ДЗ мы рассмотрим `Elastic стек (ELK)`:
  - **ElasticSearch** - TSDB и поисковый движок для хранения данных
  - **Logstash** - для агрегации и трансформации данных
  - **Kibana** - для визуализации  

Однако, для агрегации логов вместо Logstash мы будем использовать **Fluentd**, таким образом стек называется `EFK`  

- Для системы логирования создала отдельный compose-файл [docker/docker-compose-logging.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/ce683ef5c5b40ee8341b987358091ad77a5cc7ec/docker%2520docker-compose-logging.yml)
- Открыла порты в GCE
  ```
  $ gcloud compute firewall-rules create fluentd-default --allow tcp:24224,udp:24224
  $ gcloud compute firewall-rules create elasticsearch-default --allow tcp:9200,9300
  $ gcloud compute firewall-rules create kibana-default --allow tcp:5601
  ```

### Fluentd
**`Fluentd`** инструмент, который может использоваться для отправки, агрегации и преобразования лог-сообщений. Мы будем использовать его для агрегации (сбора в одной месте) и парсинга логов сервисов приложения.
- Создала диру logging/fluentd (`$ mkdir -p logging/fluentd`)
- Создала файл logging/fluentd/Dockerfile:
```sh
FROM fluent/fluentd:v0.12
RUN gem install fluent-plugin-elasticsearch --no-rdoc --no-ri --version 1.9.5
RUN gem install fluent-plugin-grok-parser --no-rdoc --no-ri --version 1.0.0
ADD fluent.conf /fluentd/etc
```
- Создала кофигурационный файл для fluentd - [logging/fluentd/fluent.conf](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/f89c99b7cef49915d718b8dcecf3adb4b5866ef8/logging%2520fluentd%2520fluent.conf)
- Соберала docker образ для fluentd (находясь в директории logging/fluentd)
  ```
  $ export USER_NAME=<my_dockerhub_login>
  $ docker build -t $USER_NAME/fluentd .
  ```

## Структурированные логи
Логи должны иметь заданную (единую) структуру и содержать необходимую для нормальной эксплуатации данного сервиса информацию о его работе  
Лог-сообщения также должны иметь понятный для выбранной системы логирования формат, чтобы избежать ненужной траты ресурсов на преобразование данных в нужный вид.  
Структурированные логи мы рассмотрим на примере сервиса post

- В файле docker/.env поменяла теги приложения на `logging`
- Запустила сервисы приложения (находясь в каталоге docker/)
  ```
  $ docker-compose up -d
  ```
- Выполнила команду для просмотра логов post сервиса:
  ```
  $ docker-compose logs -f post
  Attaching to docker_post_1
  ```
**⚠ Внимание!** Среди логов можно наблюдать проблемы с доступностью Zipkin, у нас он пока что и правда не установлен. Ошибки можно игнорировать ([Github issue](https://github.com/express42/reddit/issues/2))  

- Открыла приложение в браузере  
  http://108.59.80.183:9292/
- Создала несколько постов и пронаблюдала запись логов post:  
`post_1     | {"event": "post_create", "level": "info", "message": "Successfully created a new post", "params": {"link": "http://34.77.129.109:9292", "title": "ololol"}, "request_id": "ccf43cc0-3bbf-4436-a0ca-7bbac8e647c0", "service": "post", "timestamp": "2019-12-18 23:46:05"}`  
`post_1     | {"addr": "172.19.0.2", "event": "request", "level": "info", "method": "POST", "path": "/add_post?", "request_id": "ccf43cc0-3bbf-4436-a0ca-7bbac8e647c0", "response_status": 200, "service": "post", "timestamp": "2019-12-18 23:46:05"}`  
`post_1     | {"event": "find_all_posts", "level": "info", "message": "Successfully retrieved all posts from the database", "params": {}, "request_id": "a263bfcb-132b-4a10-9522-2922a8aa22a9", "service": "post", "timestamp": "2019-12-18 23:46:05"}`  
`post_1     | {"addr": "172.19.0.2", "event": "request", "level": "info", "method": "GET", "path": "/posts?", "request_id": "a263bfcb-132b-4a10-9522-2922a8aa22a9", "response_status": 200, "service": "post", "timestamp": "2019-12-18 23:46:05"}`
    - Каждое событие, связанное с работой приложения логируется в JSON формате и имеет структуру: 
      - **event** - тип события 
      - **message** - сообщение 
      - **params** - переданные функции параметры 
      - **service** - имя сервиса

Выключала виртуалку, ip адрес сменился, теперь так:
```
$ docker-machine regenerate-certs logging
$ eval $(docker-machine env logging)
$ docker-machine ip logging
35.223.72.229
```

### Отправка логов во Fluentd
По дефолту Docker контейнерами используется json-file драйвер для логирования информации, которая пишется сервисом внутри контейнера в **stdout** (и **stderr**). Для отправки логов во Fluentd используем [docker драйвер fluentd](https://docs.docker.com/config/containers/logging/fluentd/)  
- Определим драйвер для логирования для сервиса post в композ файле [docker/docker-compose.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/17d92b7ef415e5198e1393983be7d5bc0dcc7dfb/docker%2520docker-compose.yml)
  ```
    logging:
      driver: "fluentd"
      options:
        fluentd-address: localhost:24224
        tag: service.post
  ```  
- Поднимем инфраструктуру централизованной системы логирования и перезапустим сервисы приложения.  
  Из каталога docker:
  ```
  $ docker-compose -f docker-compose-logging.yml up -d
  $ docker-compose down
  $ docker-compose up -d
  ```

###  Что-то пошло не так
1. Не стартует кибана, тк не может достучаться до elasticsearch (судя по логам конта `docker logs -f eab17c1800b0`)

**Fix 1**  
- Зашла на хост-машину и обновила лимит памяти
  ```
  $ docker-machine ssh logging
  $ sudo su
  # sysctl -w vm.max_map_count=262144
  ```
- Пересоздала конты
  ```
  $ docker-compose -f docker-compose-logging.yml down && docker-compose -f docker-compose-logging.yml up -d
  ```

2. Эластик стартует и сразу падает с ошибкой
   ```
   ERROR: [1] bootstrap checks failed
   [1]: the default discovery settings are unsuitable for production use; at least one of [discovery.seed_hosts, discovery.seed_providers, cluster.initial_master_nodes] must be configured
   ```

**Fix 2**  
- Чот психанула и обновила версии кибаны, элестика, fluentd и его плагинов  
  Гисты на новые файлы:
    - [logging/fluentd/Dockerfile](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/17df5ffa70671d3d70bef15a5f0d9828c12b5626/logging%2520fluentd%2520Dockerfile)
    - [docker/docker-compose-logging.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/a6f5d63aeecea58cdfb17d25f0eff1a1787d0f31/docker%2520docker-compose-logging.yml%2520new1)
- Пересоздала образ fluentd и перезапустила конты
  ```
  fluentd]$ export USER_NAME=<my_dockerhub_login>
  fluentd]$ docker build -t $USER_NAME/fluentd .
  docker]$ docker-compose -f docker-compose-logging.yml down
  docker]$ docker-compose -f docker-compose-logging.yml up -d
  ```
- Хелп про сингл-ноду брала [отсюда](https://medium.com/@TimvanBaarsen/how-to-run-an-elasticsearch-7-x-single-node-cluster-for-local-development-using-docker-compose-2b7ab73d8b82)

### Kibana
**`Kibana`** - инструмент для визуализации и анализа логов от компании Elastic

- Потыкала новые посты в приложении  
  http://35.223.72.229:9292/  
- Открыла кибану  
  http://35.223.72.229:5601/  
- Настройки
    - Management/Index patterns/Create index pattern
      - Index pattern: fluentd-*
      - Time Filter field name: @timestamp
    - Тыкнуть Discover --> появится график и логи
- В левом столбце находятся названия полей. По полям можно производить поиск для быстрого нахождения нужной информации
- Сделала фильтр по `container_name: /docker_post_1`, за последние 5 минут:  
  http://35.223.72.229:5601/goto/82565ab9d966f714c6e859281e2494df
- Поле `log` содержит в себе **JSON объект**, который содержит много информации. Хотелось бы выделить эту информацию в поля, чтобы иметь возможность производить по ним поиск (например поля event, service и тд). Можно воспользоваться **фильтрами** для выделения нужной инфы
- Добавила фильтр для парсинга json логов в [logging/fluentd/fluent.conf](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/dad7da8d27d99be403f441039196e451d2dd6e1e/logging%2520fluentd%2520fluent.conf%2520new1)
  ```
  <filter service.post>
    @type parser
    format json
    key_name log
  </filter>
  ```
- Пересобрала образ и перезапустила флюент
  ```
  fluentd]$ docker build -t $USER_NAME/fluentd .
  docker]$ docker-compose -f docker-compose-logging.yml up -d fluentd
  ```
- Проверка:
  - Создала пару постов  
    http://35.223.72.229:9292/
  - Обновила кибану  
    http://35.223.72.229:5601/app/kibana#/doc/33a3b510-2403-11ea-a057-d71a3b096dd6/fluentd-20191221?id=PSsYKW8BPSH6ymNslLpB&_g=(filters:!(),refreshInterval:(pause:!t,value:0),time:(from:now-5m,to:now))
    - теперь вместо одного поля `log` появилось несколько полей `addr, event, method` и тд, по которым можно грепать. Пример `event: post_create`

## Неструктурированные логи

Неструктурированные логи отличаются отсутствием четкой структуры данных. Также часто бывает, что формат лог-сообщений не подстроен под систему централизованного логирования, что существенно увеличивает затраты вычислительных и временных ресурсов на обработку данных и выделение нужной информации.  
На примере сервиса **ui** рассмотрим пример логов с неудобным форматом сообщений.  

- По аналогии с post сервисом определим для ui сервиса драйвер для логирования `fluentd` в compose-файле [docker/docker-compose.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/61a0dadda6281c8489abb0662d026c0f2ebb4976/docker%2520docker-compose.yml%2520new2)
  ```
  logging:
     driver: "fluentd"
     options:
       fluentd-address: localhost:24224
       tag: service.ui
  ```
- Перезапустила конт
  ```
  $ docker-compose stop ui && docker-compose rm ui
  $ docker-compose up -d
  ```
- В кибане появились логи от конта ui

Когда приложение или сервис не пишет структурированные логи, приходится использовать регулярные выражения для их парсинга в [logging/fluentd/fluent.conf](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/0e89015649522af1f4b2aa66b7d0a54f6104865e/logging%2520fluentd%2520fluent.conf%2520new2)
- Эта регулярка нужна, чтобы успешно выделить интересующую нас информацию из лога UI-сервиса в поля
  ```
  <filter service.ui>
    @type parser
    format /\[(?<time>[^\]]*)\]  (?<level>\S+) (?<user>\S+)[\W]*service=(?<service>\S+)[\W]*event=(?<event>\S+)[\W]*(?:path=(?<path>\S+)[\W]*)?request_id=(?<request_id>\S+)[\W]*(?:remote_addr=(?<remote_addr>\S+)[\W]*)?(?:method= (?<method>\S+)[\W]*)?(?:response_status=(?<response_status>\S+)[\W]*)?(?:message='(?<message>[^\']*)[\W]*)?/
    key_name log
  </filter>
  ```
- Пересоздала образ и перезапустила кибану
  ```
  fluentd]$ docker build -t $USER_NAME/fluentd .
  docker]$ docker-compose -f docker-compose-logging.yml down && docker-compose -f docker-compose-logging.yml up -d
  ```

### Парсинг
Созданные регулярки могут иметь ошибки, их сложно менять и невозможно читать. Для облегчения задачи парсинга вместо стандартных регулярок можно использовать **grok-шаблоны**.  
`grok’и` - это именованные шаблоны регулярных выражений (очень похоже на функции). Можно использовать готовый regexp, просто сославшись на него как на функцию в файле logging/fluentd/fluent.conf  
- Часть логов нужно еще распарсить. Для этого используем несколько Grok-ов по-очереди в [logging/fluentd/fluent.conf](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/0ca106196b300e7f32cbabcbd0f74ccd7788a552/logging%2520fluentd%2520fluent.conf%2520new3)
- Пересобрала образ и перезапустила кибану

### Ошибка..
```
docker]$ docker-compose -f docker-compose-logging.yml logs -f fluentd

fluentd_1        | 2019-12-21 16:47:47 +0000 [info]: parsing config file is succeeded path="/fluentd/etc/fluent.conf"
fluentd_1        | 2019-12-21 16:47:47 +0000 [error]: config error file="/fluentd/etc/fluent.conf" error_class=Fluent::ConfigError error="no grok patterns. Check configuration, e.g. typo, configuration syntax, etc"
docker_fluentd_1 exited with code 1
```
- Нагуглила https://github.com/repeatedly/fluent-plugin-multi-format-parser/issues/6  
  `So if you want a working version, you have to stay on 0.12.x and force load an older version of the plugin.`
- Оооооок, вернула версию v0.12, итоговый файл [logging/fluentd/Dockerfile](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/e730b3f36de299c33e46342d53a595892be03d48/logging%2520fluentd%2520Dockerfile%2520new1)
  ```
  FROM fluent/fluentd:v0.12
  RUN fluent-gem install fluent-plugin-elasticsearch --no-rdoc --no-ri --version 1.18.1
  RUN fluent-gem install fluent-plugin-grok-parser --no-rdoc --no-ri --version 1.0.0
  ADD fluent.conf /fluentd/etc
  ```
- Пересобрала образ, перезапустила конты.
- Всё завелось

## Доп. задание №1

UI-сервис шлет логи в нескольких форматах.  
Составьте конфигурацию fluentd так, чтобы разбирались оба формата логов UI-сервиса одновременно

- Гугл в помощь - https://github.com/fluent/fluent-plugin-grok-parser
- Отредактировала `filter service.ui` в [logging/fluentd/fluent.conf](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/844254ae415db5fb845108a2207e4e52a5aef9ed/logging%2520fluentd%2520fluent.conf%2520new4)
  ```
    <grok>
      pattern service=%{WORD:service} \| event=%{WORD:event} \| request_id=%{GREEDYDATA:request_id} \| message='%{GREEDYDATA:message}'
    </grok>
    <grok>
      pattern service=%{WORD:service} \| event=%{WORD:event} \| path=%{URIPATH:path} \| request_id=%{GREEDYDATA:request_id} \| remote_addr=%{IP:remote_addr} \| method= %{WORD:message} \| response_status=%{INT:response_status}
    </grok>
  ```
- Пересобрала образ, перезапустила конты.

## Распределенный трейсинг

#### Разобраться с темой распределенного трейсинга и решить проблему в конце данного файла

### Zipkin
- Добавила в compose-файл [docker/docker-compose-logging.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/2763d9388ee3b897fda1ba811f37b8d3b751162d/docker%2520docker-compose-logging.yml%2520new2) сервис распределенного трейсинга **Zipkin**
  ```
  zipkin:
    image: openzipkin/zipkin
    ports:
      - "9411:9411"
  ```
- Прокинула порт
  ```
  $ gcloud compute firewall-rules create zipkin-default --allow tcp:9411
  ```
- В .env добавила
  ```
  ZIPKIN_ENABLED=true
  ```
- В [docker/docker-compose.yml](https://gist.githubusercontent.com/Lisskha/bb07bb4ad53cb1e684e258f025ced7fa/raw/b730246c2e6b5fb3aa3f115d0760f8a3ca686945/docker%2520docker-compose.yml%2520new3) для каждого сервиса добавтла `ENV`:
  ```
    environment:
      ZIPKIN_ENABLED: ${ZIPKIN_ENABLED}
  ```
- В файл docker-compose-logging.yml добавила определение сети для зипкина
  ```
  zipkin:
    image: openzipkin/zipkin
    ports:
      - "9411:9411"
    networks:
      - front_net
      - back_net
  ...
  networks:
    front_net:
    back_net:
  ```
- Перезапустила сервисы
  ```
  docker]$ docker-compose -f docker-compose-logging.yml -f docker-compose.yml down
  docker]$ docker-compose -f docker-compose-logging.yml -f docker-compose.yml up -d
  ```
- Открыла **Zipkin WEB UI**  
  http://35.223.72.229:9411/zipkin/
- Несколько раз обновила страницу с приложением  
  http://35.223.72.229:9292/
- Вернулась в зипкин, там появились трейсы
- Нажмем на один из трейсов, чтобы посмотреть, как запрос шел через систему микросервисов и каково время обработки запросов
  - Запрос попал к сервису ui_app, который обработал его за суммарное время 44.178ms
  - Из этих 44.178ms ушло 17.273ms на то, чтобы ui мог направить запрос post сервису по пути /posts и получить от него ответ в виде списка постов
- ***Терминология***
  - **`span`** - (синие полоски со временем) одна операция, которая произошла при обработке запроса
  - **`трейс`** - набор span-ов
  - **`Суммарное время обработки`** - равно верхнему span-у, который включает в себя время всех span-ов, расположенных под ним

## Доп. задание №2

Пользователи жалуются, что при нажатии на пост они вынуждены долго ждать, пока у них загрузится страница с постом. Жалоб на загрузку других страниц не поступало. Нужно выяснить, в чем проблема, используя Zipkin.  
[Ссылка](https://github.com/Artemmkin/bugged-code) на репозиторий со сломанным кодом приложения.


[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)


# HW 19. Введение в Kubernetes

PR:  

## Цели
- Разобрать на практике все компоненты Kubernetes, развернуть их вручную используя **The Hard Way**
- Ознакомиться с описанием основных примитивов нашего приложения и его дальнейшим запуском в Kubernetes

## Создание примитивов
Опишем приложение в контексте Kubernetes с помощью manifest-ов в YAML-формате. Основным примитивом будет *Deployment*.  
Основные задачи сущности Deployment:
- Создание Replication Controller-а (следит, чтобы число запущенных Pod-ов соответствовало описанному);
- Ведение истории версий запущенных Pod-ов (для различных стратегий деплоя, для возможностей отката);
- Описание процесса деплоя (стратегия, параметры стратегий)

Текущие файлы нужны для создания структуры и проверки работоспособности kubernetes-кластера.

- Создала директории kubernetes и kubernetes/reddit
- Файл [post-deployment.yml]() сохранила в директории kubernetes/reddit
- Создала файлы с Deployment манифестами приложений в папке kubernetes/reddit
  - [ui-deployment.yml]()
  - [comment-deployment.ym]()
  - [mongo-deployment.yml]()

**P.S.** Эту директорию и файлы в ней в дальнейшем мы будем развивать (пока это нерабочие экземпляры).

## Kubernetes The Hard Way

В качестве домашнего задания предлагается пройти [Kubernetes The Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way), разработанный инженером Google Kelsey Hightower  
Туториал представляет собой:
- Пошаговое руководство по ручной инсталляции основных компонентов Kubernetes кластера;
- Краткое описание необходимых действий и объектов

### Задание
- Создать диру kubernetes/the_hard_way
- Пройти Kubernetes The Hard Way
- Проверить, что `kubectl apply -f <filename>` проходит по созданным до этого deployment-ам (ui, post, mongo, comment) и поды запускаются
- Удалить кластер после прохождения THW
- Все, созданные в ходе прохождения THW файлы (кроме бинарных) поместить в папку **kubernetes/the_hard_way** репозитория (сертификаты и ключи тоже можно коммитить, но только после удаления кластера)

### Возможные проблемы
- Если на шаге **Bootstrapping the etcd Cluster** у вас не работает команда `sudo systemctl start etcd`, то, вероятно, Вы не используете параллельный ввод с помощью tmux, а выполняете команды для каждого сервера отдельно. Для того, чтобы команда выполнилась успешно, установите etcd на каждый необходимый инстанс и одновременно запустите её на всех инстансах.

- Если в процессе выполнения команд возникает ошибка `(gcloud.compute.addresses.describe) argument --region: expected one argument`, то убедитесь, что Вы выполняете команду в нужном месте. Обычно это происходит, когда команду необходимо выполнять на локальной машине, а она выполняется на каком то из инстансов. Если команда точно выполняется локально, то выполните:
```
{
  gcloud config set compute/region us-west1
  gcloud config set compute/zone us-west1-c
}
```

## **Kubernetes THW**

## Cluster Details
Kubernetes The Hard Way guides you through bootstrapping a highly available Kubernetes cluster with end-to-end encryption between components and RBAC authentication.
- kubernetes 1.15.3
- containerd 1.2.9
- coredns v1.6.3
- cni v0.7.1
- etcd v3.4.0

## Prerequisites

```
$ gcloud version
Google Cloud SDK 263.0.0
bq 2.0.47
core 2019.09.13
gsutil 4.42
```
- Проинициализировать и залогиниться в Google Cloud SDK, поменять дефолтные настройки региона и зоны
  ```sh
  $ gcloud init
  $ gcloud auth login
  $ gcloud config set compute/region us-west1
  $ gcloud config set compute/zone us-west1-c

  # так можно посмотреть доступные зоны
  $ gcloud compute zones list
  ```

## Installing the Client Tools

- Полезные туториалы: [cfssl](https://github.com/cloudflare/cfssl), [cfssljson](https://github.com/cloudflare/cfssl), [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

### Install CFSSL
`cfssl` и `cfssljson` будут использоваться для провижинга [PKI Infrastructure](https://en.wikipedia.org/wiki/Public_key_infrastructure) и для генерации TLS сертов

- For OS X
  ```sh
  $ brew install cfssl

  $ cfssl version
  Version: 1.4.1
  Runtime: go1.13.4

  $ cfssljson --version
  Version: 1.4.1
  Runtime: go1.13.4
  ```
- For Linux
  ```sh
  wget -q --show-progress --https-only --timestamping \
  https://storage.googleapis.com/kubernetes-the-hard-way/cfssl/linux/cfssl \
  https://storage.googleapis.com/kubernetes-the-hard-way/cfssl/linux/cfssljson

  chmod +x cfssl cfssljson
  sudo mv cfssl cfssljson /usr/local/bin/
  ```

### Install kubectl
- For OS X
  ```sh
  curl -o kubectl https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/darwin/amd64/kubectl
  
  chmod +x kubectl
  sudo mv kubectl /usr/local/bin/
  ```
- For Linux
  ```sh
  wget https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/linux/amd64/kubectl

  chmod +x kubectl
  sudo mv kubectl /usr/local/bin/
  ```
- У меня уже был установлен, просто проверила версию:
  ```sh
  $ kubectl version --client
  Client Version: version.Info{Major:"1", Minor:"15", GitVersion:"v1.15.2", GitCommit:"f6278300bebbb750328ac16ee6dd3aa7d3549568", GitTreeState:"clean", BuildDate:"2019-08-05T16:54:35Z", GoVersion:"go1.12.7", Compiler:"gc", Platform:"darwin/amd64"}
  ```

## Provisioning Compute Resources

В этой лабе будем запускать кластер Kubernetes в одной зоне.  

### Networking
The Kubernetes [networking model](https://kubernetes.io/docs/concepts/cluster-administration/networking/#kubernetes-model) assumes a flat network in which containers and nodes can communicate with each other.  
In cases where this is not desired [network policies](https://kubernetes.io/docs/concepts/services-networking/network-policies/) can limit how groups of containers are allowed to communicate with each other and external network endpoints.  

**`Virtual Private Cloud (VPC) Network`**  
- Создала VPC `kubernetes-the-hard-way`
  ```sh
  $ gcloud compute networks create kubernetes-the-hard-way --subnet-mode custom
  ```
- Из назначенной подсети будут выдаваться IP адреса каждой ноде в кластере кубика. Создала подсеть `kubernetes` в VPC `kubernetes-the-hard-way`
  ```sh
  $ gcloud compute networks subnets create kubernetes \
    --network kubernetes-the-hard-way \
    --range 10.240.0.0/24

  NAME        REGION    NETWORK                  RANGE
  kubernetes  us-west1  kubernetes-the-hard-way  10.240.0.0/24
  ```
> The 10.240.0.0/24 IP address range can host up to 254 compute instances.  

**`Firewall Rules`**  
- Создала правило фаерволла, которое разрешает внутреннюю связь по всем протоколам
  ```sh
  gcloud compute firewall-rules create kubernetes-the-hard-way-allow-internal \
  --allow tcp,udp,icmp \
  --network kubernetes-the-hard-way \
  --source-ranges 10.240.0.0/24,10.200.0.0/16
  ```
- Правило для SSH, ICMP, and HTTPS
  ```sh
  gcloud compute firewall-rules create kubernetes-the-hard-way-allow-external \
  --allow tcp:22,tcp:6443,icmp \
  --network kubernetes-the-hard-way \
  --source-ranges 0.0.0.0/0
  ```
- Проверка созданных правил
  ```sh
  $ gcloud compute firewall-rules list --filter="network:kubernetes-the-hard-way"

  NAME                                    NETWORK                  DIRECTION  PRIORITY  ALLOW                 DENY  DISABLED
  kubernetes-the-hard-way-allow-external  kubernetes-the-hard-way  INGRESS    1000      tcp:22,tcp:6443,icmp        False
  kubernetes-the-hard-way-allow-internal  kubernetes-the-hard-way  INGRESS    1000      tcp,udp,icmp                False
  ```

**`Kubernetes Public IP Address`**  

- Выделить статик IP в своем регионе
  ```sh
  $ gcloud compute addresses create kubernetes-the-hard-way \
  --region $(gcloud config get-value compute/region)
  ```
- И проверить
  ```sh
  $ gcloud compute addresses list --filter="name=('kubernetes-the-hard-way')"
  NAME                     ADDRESS/RANGE   TYPE      REGION    STATUS
  kubernetes-the-hard-way  104.198.101.88  EXTERNAL  us-west1  RESERVED
  ```

### Compute Instances
- `Kubernetes Controllers`
  - Создать три инстанса
  ```sh
  for i in 0 1 2; do
  gcloud compute instances create controller-${i} \
    --async \
    --boot-disk-size 200GB \
    --can-ip-forward \
    --image-family ubuntu-1804-lts \
    --image-project ubuntu-os-cloud \
    --machine-type n1-standard-1 \
    --private-network-ip 10.240.0.1${i} \
    --scopes compute-rw,storage-ro,service-management,service-control,logging-write,monitoring \
    --subnet kubernetes \
    --tags kubernetes-the-hard-way,controller
  done
  ```
- `Kubernetes Workers`
  - Создать три инстанса под воркеры
  ```sh
  for i in 0 1 2; do
  gcloud compute instances create worker-${i} \
    --async \
    --boot-disk-size 200GB \
    --can-ip-forward \
    --image-family ubuntu-1804-lts \
    --image-project ubuntu-os-cloud \
    --machine-type n1-standard-1 \
    --metadata pod-cidr=10.200.${i}.0/24 \
    --private-network-ip 10.240.0.2${i} \
    --scopes compute-rw,storage-ro,service-management,service-control,logging-write,monitoring \
    --subnet kubernetes \
    --tags kubernetes-the-hard-way,worker
  done
  ```
> Each worker instance requires a pod subnet allocation from the Kubernetes cluster CIDR range. The pod subnet allocation will be used to configure container networking in a later exercise. The **pod-cidr** instance metadata will be used to expose pod subnet allocations to compute instances at runtime.

> The Kubernetes cluster CIDR range is defined by the Controller Manager's --cluster-cidr flag. In this tutorial the cluster CIDR range will be set to 10.200.0.0/16, which supports 254 subnets.

- `Verification`
  - Смотрим список инстансов в нашей зоне
  ```sh
  $ gcloud compute instances list

  NAME           ZONE            MACHINE_TYPE   PREEMPTIBLE  INTERNAL_IP  EXTERNAL_IP     STATUS
  controller-0   us-west1-c      n1-standard-1               10.240.0.10  35.247.11.112   RUNNING
  controller-1   us-west1-c      n1-standard-1               10.240.0.11  35.185.196.1    RUNNING
  controller-2   us-west1-c      n1-standard-1               10.240.0.12  35.247.115.224  RUNNING
  worker-0       us-west1-c      n1-standard-1               10.240.0.20  35.197.116.118  RUNNING
  worker-1       us-west1-c      n1-standard-1               10.240.0.21  35.199.149.150  RUNNING
  worker-2       us-west1-c      n1-standard-1               10.240.0.22  35.197.104.4    RUNNING
  ```

### Configuring SSH Access
- Создается ключ и складывается в метадату
  ```sh
  $ gcloud compute ssh controller-0
  ```


## Provisioning a CA and Generating TLS Certificates

### Certificate Authority  
<details>
<summary> Генерим CA конф файл, серт и приватный ключ</summary>
<p>
 
```sh
$ cat > ca-config.json <<EOF
{
  "signing": {
    "default": {
      "expiry": "8760h"
    },
    "profiles": {
      "kubernetes": {
        "usages": ["signing", "key encipherment", "server auth", "client auth"],
        "expiry": "8760h"
      }
    }
  }
}
EOF

$ cat > ca-csr.json <<EOF
{
  "CN": "Kubernetes",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "Kubernetes",
      "OU": "CA",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
$ cfssl gencert -initca ca-csr.json | cfssljson -bare ca

# Результат
$ ll
-rw-------    ca-key.pem
-rw-r--r--    ca.pem
```
</p>
</details> 

### Client and Server Certificates
Генерим клиентские и серверные сертификаты для каждого компонента Kubernetes и клиентский сертификат для админа Kubernetes
  
<details>
<summary> The Admin Client Certificate </summary>
<p>

```sh
cat > admin-csr.json <<EOF
{
  "CN": "admin",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "system:masters",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -profile=kubernetes \
  admin-csr.json | cfssljson -bare admin

# Результат
-rw-------   admin-key.pem
-rw-r--r--   admin.pem
```

</p>
</details>  

<details>
<summary> The Kubelet Client Certificates </summary>
<p>

```sh
for instance in worker-0 worker-1 worker-2; do
cat > ${instance}-csr.json <<EOF
{
  "CN": "system:node:${instance}",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "system:nodes",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

EXTERNAL_IP=$(gcloud compute instances describe ${instance} \
  --format 'value(networkInterfaces[0].accessConfigs[0].natIP)')

INTERNAL_IP=$(gcloud compute instances describe ${instance} \
  --format 'value(networkInterfaces[0].networkIP)')

cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -hostname=${instance},${EXTERNAL_IP},${INTERNAL_IP} \
  -profile=kubernetes \
  ${instance}-csr.json | cfssljson -bare ${instance}
done

# Результат
-rw-------   worker-0-key.pem
-rw-r--r--   worker-0.pem
-rw-------   worker-1-key.pem
-rw-r--r--   worker-1.pem
-rw-------   worker-2-key.pem
-rw-r--r--   worker-2.pem
```

</p>
</details>  

<details>
<summary> The Controller Manager Client Certificate </summary>
<p>

```sh
cat > kube-controller-manager-csr.json <<EOF
{
  "CN": "system:kube-controller-manager",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "system:kube-controller-manager",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -profile=kubernetes \
  kube-controller-manager-csr.json | cfssljson -bare kube-controller-manager

# Результат
-rw-------   kube-controller-manager-key.pem
-rw-r--r--   kube-controller-manager.pem
```

</p>
</details>  

<details>
<summary> The Kube Proxy Client Certificate </summary>
<p>

```sh
cat > kube-proxy-csr.json <<EOF
{
  "CN": "system:kube-proxy",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "system:node-proxier",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -profile=kubernetes \
  kube-proxy-csr.json | cfssljson -bare kube-proxy

# Результат
-rw-------   kube-proxy-key.pem
-rw-r--r--   kube-proxy.pem
```

</p>
</details>  

<details>
<summary> The Scheduler Client Certificate </summary>
<p>

```sh
cat > kube-scheduler-csr.json <<EOF
{
  "CN": "system:kube-scheduler",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "system:kube-scheduler",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -profile=kubernetes \
  kube-scheduler-csr.json | cfssljson -bare kube-scheduler

# Результат
-rw-------   kube-scheduler-key.pem
-rw-r--r--   kube-scheduler.pem
```

</p>
</details>  

<details>
<summary> The Kubernetes API Server Certificate </summary>
<p>

```sh
# Вытащить статик ип из GCE
KUBERNETES_PUBLIC_ADDRESS=$(gcloud compute addresses describe kubernetes-the-hard-way \
  --region $(gcloud config get-value compute/region) \
  --format 'value(address)')

KUBERNETES_HOSTNAMES=kubernetes,kubernetes.default,kubernetes.default.svc,kubernetes.default.svc.cluster,kubernetes.svc.cluster.local

cat > kubernetes-csr.json <<EOF
{
  "CN": "kubernetes",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "Kubernetes",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -hostname=10.32.0.1,10.240.0.10,10.240.0.11,10.240.0.12,${KUBERNETES_PUBLIC_ADDRESS},127.0.0.1,${KUBERNETES_HOSTNAMES} \
  -profile=kubernetes \
  kubernetes-csr.json | cfssljson -bare kubernetes

# Результат
-rw-------   kubernetes-key.pem
-rw-r--r--   kubernetes.pem
```

</p>
</details> 

> The kubernetes-the-hard-way static IP address will be included in the list of subject alternative names for the Kubernetes API Server certificate. This will ensure the certificate can be validated by remote clients.  

> The Kubernetes API server is automatically assigned the kubernetes internal dns name, which will be linked to the first IP address (10.32.0.1) from the address range (10.32.0.0/24) reserved for internal cluster services during the [control plane bootstrapping](https://github.com/kelseyhightower/kubernetes-the-hard-way/blob/master/docs/08-bootstrapping-kubernetes-controllers.md#configure-the-kubernetes-api-server) lab.

<details>
<summary> The Service Account Key Pair </summary>
<p>

```sh
cat > service-account-csr.json <<EOF
{
  "CN": "service-accounts",
  "key": {
    "algo": "rsa",
    "size": 2048
  },
  "names": [
    {
      "C": "US",
      "L": "Portland",
      "O": "Kubernetes",
      "OU": "Kubernetes The Hard Way",
      "ST": "Oregon"
    }
  ]
}
EOF

# Генерим серт и ключ
cfssl gencert \
  -ca=ca.pem \
  -ca-key=ca-key.pem \
  -config=ca-config.json \
  -profile=kubernetes \
  service-account-csr.json | cfssljson -bare service-account

# Результат
-rw-------   service-account-key.pem
-rw-r--r--   service-account.pem
```

</p>
</details>  

### Distribute the Client and Server Certificates
- Копируем серты и ключи на воркеры
```sh
for instance in worker-0 worker-1 worker-2; do
  gcloud compute scp ca.pem ${instance}-key.pem ${instance}.pem ${instance}:~/
done
```
- Копируем серты и ключи на контроллеры
```sh
for instance in controller-0 controller-1 controller-2; do
  gcloud compute scp ca.pem ca-key.pem kubernetes-key.pem kubernetes.pem \
    service-account-key.pem service-account.pem ${instance}:~/
done
```

> The kube-proxy, kube-controller-manager, kube-scheduler, and kubelet client certificates will be used to generate client authentication configuration files in the next lab.

## Generating Kubernetes Configuration Files for Authentication

### Client Authentication Configs
Будем генерить kubeconfig файлы для `controller manager`, `kubelet`, `kube-proxy`, планировщика и админа.  
- **`Kubernetes Public IP Address`**  
  Каждому kubeconfig нужно канекаться к Kubernetes API Server. Для доступности заасайним статик ip на внешний LB за которым будет Kubernetes API Servers
    - Извлечь статик IP
      ```sh
      KUBERNETES_PUBLIC_ADDRESS=$(gcloud compute addresses describe kubernetes-the-hard-way \
      --region $(gcloud config get-value compute/region) \
      --format 'value(address)')
      ```
- **`The kubelet Kubernetes Configuration File`**  
  При создании файлов kubeconfig для Kubelets должен использоваться сертификат клиента, соответствующий имени узла Kubelet. Тогда будет норм работать Kubernetes [Node Authorizer](https://kubernetes.io/docs/reference/access-authn-authz/node/)  
  > Команды нужно запускать в той же дире, где генерили серты в разделе [Provisioning a CA and Generating TLS Certificates](#Provisioning-a-CA-and-Generating-TLS-Certificates) 
    - Генерация kubeconfig файлов для каждого воркера
      ```sh
      for instance in worker-0 worker-1 worker-2; do kubectl config set-cluster kubernetes-the-hard-way \
      --certificate-authority=ca.pem \
      --embed-certs=true \
      --server=https://${KUBERNETES_PUBLIC_ADDRESS}:6443 \
      --kubeconfig=${instance}.kubeconfig

      kubectl config set-credentials system:node:${instance} \
      --client-certificate=${instance}.pem \
      --client-key=${instance}-key.pem \
      --embed-certs=true \
      --kubeconfig=${instance}.kubeconfig

      kubectl config set-context default \
      --cluster=kubernetes-the-hard-way \
      --user=system:node:${instance} \
      --kubeconfig=${instance}.kubeconfig

      kubectl config use-context default --kubeconfig=${instance}.kubeconfig
      done
      ```
    - Создались файлы
      ```
      -rw-------   worker-0.kubeconfig
      -rw-------   worker-1.kubeconfig
      -rw-------   worker-2.kubeconfig
      ```
- **`The kube-proxy Kubernetes Configuration File`**
  - Генерация kubeconfig файла для kube-proxy
    ```sh
    kubectl config set-cluster kubernetes-the-hard-way \
    --certificate-authority=ca.pem \
    --embed-certs=true \
    --server=https://${KUBERNETES_PUBLIC_ADDRESS}:6443 \
    --kubeconfig=kube-proxy.kubeconfig

    kubectl config set-credentials system:kube-proxy \
    --client-certificate=kube-proxy.pem \
    --client-key=kube-proxy-key.pem \
    --embed-certs=true \
    --kubeconfig=kube-proxy.kubeconfig

    kubectl config set-context default \
    --cluster=kubernetes-the-hard-way \
    --user=system:kube-proxy \
    --kubeconfig=kube-proxy.kubeconfig

    kubectl config use-context default --kubeconfig=kube-proxy.kubeconfig
    ``` 
  - Создался файл
    ```
    -rw-------   kube-proxy.kubeconfig
    ```
- **`The kube-controller-manager Kubernetes Configuration File`**
  - Генерим kubeconfig для kube-controller-manager
    ```sh
    kubectl config set-cluster kubernetes-the-hard-way \
    --certificate-authority=ca.pem \
    --embed-certs=true \
    --server=https://127.0.0.1:6443 \
    --kubeconfig=kube-controller-manager.kubeconfig

    kubectl config set-credentials system:kube-controller-manager \
    --client-certificate=kube-controller-manager.pem \
    --client-key=kube-controller-manager-key.pem \
    --embed-certs=true \
    --kubeconfig=kube-controller-manager.kubeconfig

    kubectl config set-context default \
    --cluster=kubernetes-the-hard-way \
    --user=system:kube-controller-manager \
    --kubeconfig=kube-controller-manager.kubeconfig

    kubectl config use-context default --kubeconfig=kube-controller-manager.kubeconfig
    ```
  - Файл готов
    ```
    -rw-------   kube-controller-manager.kubeconfig
    ```
- **`The kube-scheduler Kubernetes Configuration File`**
  - Генерим kubeconfig для kube-scheduler
    ```sh
    kubectl config set-cluster kubernetes-the-hard-way \
    --certificate-authority=ca.pem \
    --embed-certs=true \
    --server=https://127.0.0.1:6443 \
    --kubeconfig=kube-scheduler.kubeconfig

    kubectl config set-credentials system:kube-scheduler \
    --client-certificate=kube-scheduler.pem \
    --client-key=kube-scheduler-key.pem \
    --embed-certs=true \
    --kubeconfig=kube-scheduler.kubeconfig

    kubectl config set-context default \
    --cluster=kubernetes-the-hard-way \
    --user=system:kube-scheduler \
    --kubeconfig=kube-scheduler.kubeconfig

    kubectl config use-context default --kubeconfig=kube-scheduler.kubeconfig
    ```
  - Файл готов
    ```
    -rw-------   kube-scheduler.kubeconfig
    ```
- **`The admin Kubernetes Configuration File`**
  - Генерим kubeconfig для админа
    ```sh
    kubectl config set-cluster kubernetes-the-hard-way \
    --certificate-authority=ca.pem \
    --embed-certs=true \
    --server=https://127.0.0.1:6443 \
    --kubeconfig=admin.kubeconfig

    kubectl config set-credentials admin \
    --client-certificate=admin.pem \
    --client-key=admin-key.pem \
    --embed-certs=true \
    --kubeconfig=admin.kubeconfig

    kubectl config set-context default \
    --cluster=kubernetes-the-hard-way \
    --user=admin \
    --kubeconfig=admin.kubeconfig

    kubectl config use-context default --kubeconfig=admin.kubeconfig
    ```
  - Файл готов
    ```
    -rw-------   admin.kubeconfig
    ```

### Distribute the Kubernetes Configuration Files
- Копируем кубеконфиги kubelet и kube-proxy на воркеры
```sh
for instance in worker-0 worker-1 worker-2; do
  gcloud compute scp ${instance}.kubeconfig kube-proxy.kubeconfig ${instance}:~/
done
```
- Копируем кубеконфиги admin, kube-controller-manager и kube-scheduler на контроллеры
```sh
for instance in controller-0 controller-1 controller-2; do
  gcloud compute scp admin.kubeconfig kube-controller-manager.kubeconfig kube-scheduler.kubeconfig ${instance}:~/
done
```

## Generating the Data Encryption Config and Key
Kubernetes хранит различные данные, включая состояние кластера, конфиги приложенией и секреты. Kubernetes поддерживает возможность [шифрования данных](https://kubernetes.io/docs/tasks/administer-cluster/encrypt-data/) кластера в состоянии покоя.  
Создадим ключ шифрования и [encryption config](https://kubernetes.io/docs/tasks/administer-cluster/encrypt-data/#understanding-the-encryption-at-rest-configuration), подходящие для шифрования Kubernetes Secrets 

### The Encryption Key
```sh
ENCRYPTION_KEY=$(head -c 32 /dev/urandom | base64)
```
### The Encryption Config File
- Создали файл `encryption-config.yaml`
```sh
cat > encryption-config.yaml <<EOF
kind: EncryptionConfig
apiVersion: v1
resources:
  - resources:
      - secrets
    providers:
      - aescbc:
          keys:
            - name: key1
              secret: ${ENCRYPTION_KEY}
      - identity: {}
EOF
```
- И скопировали его на контроллеры
```sh
for instance in controller-0 controller-1 controller-2; do
  gcloud compute scp encryption-config.yaml ${instance}:~/
done
```

## Bootstrapping the etcd Cluster
Kubernetes components are stateless and store cluster state in [etcd](https://github.com/etcd-io/etcd). We will bootstrap a three node etcd cluster and configure it for high availability and secure remote access.

### Prerequisites
> Все дальнейшие команды нужно запускать на каждом инстансе: `controller-0`, `controller-1`, and `controller-2`
- Логинимся на контроллеры
```sh
$ gcloud compute ssh controller-0
$ gcloud compute ssh controller-1
$ gcloud compute ssh controller-2
```
### Bootstrapping an etcd Cluster Member
- Качаем официальные [etcd release binaries](https://github.com/etcd-io/etcd/releases) с GitHub
  ```sh
  wget -q --show-progress --https-only --timestamping \
  "https://github.com/etcd-io/etcd/releases/download/v3.4.0/etcd-v3.4.0-linux-amd64.tar.gz"
  ```
- Разархивируем и устанавливаем `etcd server` и `etcdctl`
  ```sh
  tar -xvf etcd-v3.4.0-linux-amd64.tar.gz
  sudo mv etcd-v3.4.0-linux-amd64/etcd* /usr/local/bin/
  ```
- Конфигурим etcd server
  ```sh
  sudo mkdir -p /etc/etcd /var/lib/etcd
  sudo cp ca.pem kubernetes-key.pem kubernetes.pem /etc/etcd/
  ```
  - The instance internal IP address will be used to serve client requests and communicate with etcd cluster peers. Retrieve the internal IP address for the current compute instance
  ```sh
  INTERNAL_IP=$(curl -s -H "Metadata-Flavor: Google" \
  http://metadata.google.internal/computeMetadata/v1/instance/network-interfaces/0/ip)
  ```
  - Each etcd member must have a unique name within an etcd cluster. Set the etcd name to match the hostname of the current compute instance
  ```sh
  ETCD_NAME=$(hostname -s)
  ```
  - Создаем systemd unit `etcd.service` и стартуем etcd server

<details>
<summary> etcd.service</summary>
<p>

```sh
cat <<EOF | sudo tee /etc/systemd/system/etcd.service
[Unit]
Description=etcd
Documentation=https://github.com/coreos

[Service]
Type=notify
ExecStart=/usr/local/bin/etcd \\
  --name ${ETCD_NAME} \\
  --cert-file=/etc/etcd/kubernetes.pem \\
  --key-file=/etc/etcd/kubernetes-key.pem \\
  --peer-cert-file=/etc/etcd/kubernetes.pem \\
  --peer-key-file=/etc/etcd/kubernetes-key.pem \\
  --trusted-ca-file=/etc/etcd/ca.pem \\
  --peer-trusted-ca-file=/etc/etcd/ca.pem \\
  --peer-client-cert-auth \\
  --client-cert-auth \\
  --initial-advertise-peer-urls https://${INTERNAL_IP}:2380 \\
  --listen-peer-urls https://${INTERNAL_IP}:2380 \\
  --listen-client-urls https://${INTERNAL_IP}:2379,https://127.0.0.1:2379 \\
  --advertise-client-urls https://${INTERNAL_IP}:2379 \\
  --initial-cluster-token etcd-cluster-0 \\
  --initial-cluster controller-0=https://10.240.0.10:2380,controller-1=https://10.240.0.11:2380,controller-2=https://10.240.0.12:2380 \\
  --initial-cluster-state new \\
  --data-dir=/var/lib/etcd
Restart=on-failure
RestartSec=5

[Install]
WantedBy=multi-user.target
EOF
```

</p>
</details>  

```sh
sudo systemctl daemon-reload
sudo systemctl enable etcd
sudo systemctl start etcd
```

### Verification
- List the etcd cluster members
```sh
sudo ETCDCTL_API=3 etcdctl member list \
  --endpoints=https://127.0.0.1:2379 \
  --cacert=/etc/etcd/ca.pem \
  --cert=/etc/etcd/kubernetes.pem \
  --key=/etc/etcd/kubernetes-key.pem
```
> output
```sh
3a57933972cb5131, started, controller-2, https://10.240.0.12:2380, https://10.240.0.12:2379, false
f98dc20bce6225a0, started, controller-0, https://10.240.0.10:2380, https://10.240.0.10:2379, false
ffed16798470cab5, started, controller-1, https://10.240.0.11:2380, https://10.240.0.11:2379, false
```

## Bootstrapping the Kubernetes Control Plane
In this lab you will bootstrap the Kubernetes control plane across three compute instances and configure it for high availability. You will also create an external load balancer that exposes the Kubernetes API Servers to remote clients. The following components will be installed on each node: Kubernetes API Server, Scheduler, and Controller Manager.

### Prerequisites
> Все дальнейшие команды нужно запускать на каждом инстансе: `controller-0`, `controller-1`, and `controller-2`
- Логинимся на контроллеры
```sh
$ gcloud compute ssh controller-0
$ gcloud compute ssh controller-1
$ gcloud compute ssh controller-2
```

### Provision the Kubernetes Control Plane
- Create the Kubernetes configuration directory  
  `sudo mkdir -p /etc/kubernetes/config`
- Download the official Kubernetes release binaries
```sh
wget -q --show-progress --https-only --timestamping \
  "https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/linux/amd64/kube-apiserver" \
  "https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/linux/amd64/kube-controller-manager" \
  "https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/linux/amd64/kube-scheduler" \
  "https://storage.googleapis.com/kubernetes-release/release/v1.15.3/bin/linux/amd64/kubectl"
```
- Install the Kubernetes binaries
```sh
chmod +x kube-apiserver kube-controller-manager kube-scheduler kubectl
sudo mv kube-apiserver kube-controller-manager kube-scheduler kubectl /usr/local/bin/
```

**`Configure the Kubernetes API Server`**
```sh
sudo mkdir -p /var/lib/kubernetes/
sudo mv ca.pem ca-key.pem kubernetes-key.pem kubernetes.pem \
service-account-key.pem service-account.pem \
encryption-config.yaml /var/lib/kubernetes/
```
- The instance internal IP address will be used to advertise the API Server to members of the cluster. Retrieve the internal IP address for the current compute instance
```sh
INTERNAL_IP=$(curl -s -H "Metadata-Flavor: Google" \
http://metadata.google.internal/computeMetadata/v1/instance/network-interfaces/0/ip)
```
- Create the kube-apiserver.service systemd unit file

<details>
<summary> kube-apiserver.service </summary>
<p>

```sh
cat <<EOF | sudo tee /etc/systemd/system/kube-apiserver.service
[Unit]
Description=Kubernetes API Server
Documentation=https://github.com/kubernetes/kubernetes

[Service]
ExecStart=/usr/local/bin/kube-apiserver \\
  --advertise-address=${INTERNAL_IP} \\
  --allow-privileged=true \\
  --apiserver-count=3 \\
  --audit-log-maxage=30 \\
  --audit-log-maxbackup=3 \\
  --audit-log-maxsize=100 \\
  --audit-log-path=/var/log/audit.log \\
  --authorization-mode=Node,RBAC \\
  --bind-address=0.0.0.0 \\
  --client-ca-file=/var/lib/kubernetes/ca.pem \\
  --enable-admission-plugins=NamespaceLifecycle,NodeRestriction,LimitRanger,ServiceAccount,DefaultStorageClass,ResourceQuota \\
  --etcd-cafile=/var/lib/kubernetes/ca.pem \\
  --etcd-certfile=/var/lib/kubernetes/kubernetes.pem \\
  --etcd-keyfile=/var/lib/kubernetes/kubernetes-key.pem \\
  --etcd-servers=https://10.240.0.10:2379,https://10.240.0.11:2379,https://10.240.0.12:2379 \\
  --event-ttl=1h \\
  --encryption-provider-config=/var/lib/kubernetes/encryption-config.yaml \\
  --kubelet-certificate-authority=/var/lib/kubernetes/ca.pem \\
  --kubelet-client-certificate=/var/lib/kubernetes/kubernetes.pem \\
  --kubelet-client-key=/var/lib/kubernetes/kubernetes-key.pem \\
  --kubelet-https=true \\
  --runtime-config=api/all \\
  --service-account-key-file=/var/lib/kubernetes/service-account.pem \\
  --service-cluster-ip-range=10.32.0.0/24 \\
  --service-node-port-range=30000-32767 \\
  --tls-cert-file=/var/lib/kubernetes/kubernetes.pem \\
  --tls-private-key-file=/var/lib/kubernetes/kubernetes-key.pem \\
  --v=2
Restart=on-failure
RestartSec=5

[Install]
WantedBy=multi-user.target
EOF
```

</p>
</details>  

**`Configure the Kubernetes Controller Manager`**  
- Move the kube-controller-manager kubeconfig into place and create the `kube-controller-manager.service` systemd unit file
```sh
sudo mv kube-controller-manager.kubeconfig /var/lib/kubernetes/
```
<details>
<summary> kube-controller-manager.service </summary>
<p>

```sh
cat <<EOF | sudo tee /etc/systemd/system/kube-controller-manager.service
[Unit]
Description=Kubernetes Controller Manager
Documentation=https://github.com/kubernetes/kubernetes

[Service]
ExecStart=/usr/local/bin/kube-controller-manager \\
  --address=0.0.0.0 \\
  --cluster-cidr=10.200.0.0/16 \\
  --cluster-name=kubernetes \\
  --cluster-signing-cert-file=/var/lib/kubernetes/ca.pem \\
  --cluster-signing-key-file=/var/lib/kubernetes/ca-key.pem \\
  --kubeconfig=/var/lib/kubernetes/kube-controller-manager.kubeconfig \\
  --leader-elect=true \\
  --root-ca-file=/var/lib/kubernetes/ca.pem \\
  --service-account-private-key-file=/var/lib/kubernetes/service-account-key.pem \\
  --service-cluster-ip-range=10.32.0.0/24 \\
  --use-service-account-credentials=true \\
  --v=2
Restart=on-failure
RestartSec=5

[Install]
WantedBy=multi-user.target
EOF
```

</p>
</details>  

**`Configure the Kubernetes Scheduler`**  
- Move the kube-scheduler kubeconfig into place and create the `kube-scheduler.yaml` configuration file
```sh
sudo mv kube-scheduler.kubeconfig /var/lib/kubernetes/
```
```sh
cat <<EOF | sudo tee /etc/kubernetes/config/kube-scheduler.yaml
apiVersion: kubescheduler.config.k8s.io/v1alpha1
kind: KubeSchedulerConfiguration
clientConnection:
  kubeconfig: "/var/lib/kubernetes/kube-scheduler.kubeconfig"
leaderElection:
  leaderElect: true
EOF
```
- Create the `kube-scheduler.service` systemd unit file
```sh
cat <<EOF | sudo tee /etc/systemd/system/kube-scheduler.service
[Unit]
Description=Kubernetes Scheduler
Documentation=https://github.com/kubernetes/kubernetes

[Service]
ExecStart=/usr/local/bin/kube-scheduler \\
  --config=/etc/kubernetes/config/kube-scheduler.yaml \\
  --v=2
Restart=on-failure
RestartSec=5

[Install]
WantedBy=multi-user.target
EOF
```

**`Start the Controller Services`**  
```sh
sudo systemctl daemon-reload
sudo systemctl enable kube-apiserver kube-controller-manager kube-scheduler
sudo systemctl start kube-apiserver kube-controller-manager kube-scheduler
```

### Enable HTTP Health Checks

A [Google Network Load Balancer](https://cloud.google.com/load-balancing/docs/network/) will be used to distribute traffic across the three API servers and allow each API server to terminate TLS connections and validate client certificates. The network load balancer only supports HTTP health checks which means the HTTPS endpoint exposed by the API server cannot be used. As a workaround the nginx webserver can be used to proxy HTTP health checks. In this section nginx will be installed and configured to accept HTTP health checks on port 80 and proxy the connections to the API server on https://127.0.0.1:6443/healthz  

> The /healthz API server endpoint does not require authentication by default  

Установим базовый веб-сервер для хелсчеков
```sh
sudo apt-get update
sudo apt-get install -y nginx
```
```sh
cat > kubernetes.default.svc.cluster.local <<EOF
server {
  listen      80;
  server_name kubernetes.default.svc.cluster.local;

  location /healthz {
     proxy_pass                    https://127.0.0.1:6443/healthz;
     proxy_ssl_trusted_certificate /var/lib/kubernetes/ca.pem;
  }
}
EOF
```
```sh
sudo mv kubernetes.default.svc.cluster.local \
    /etc/nginx/sites-available/kubernetes.default.svc.cluster.local

sudo ln -s /etc/nginx/sites-available/kubernetes.default.svc.cluster.local /etc/nginx/sites-enabled/
```
```sh
sudo systemctl restart nginx
sudo systemctl enable nginx
```
**`Verification`**
На каждом контроллере проверяем статус
```sh
kubectl get cs --kubeconfig admin.kubeconfig

NAME                 STATUS    MESSAGE             ERROR
scheduler            Healthy   ok
etcd-1               Healthy   {"health":"true"}
controller-manager   Healthy   ok
etcd-0               Healthy   {"health":"true"}
etcd-2               Healthy   {"health":"true"}
```
Проверяем хелсчеки (тоже на контроллерах)
```sh
curl -H "Host: kubernetes.default.svc.cluster.local" -i http://127.0.0.1/healthz

HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Sun, 05 Jan 2020 01:44:07 GMT
Content-Type: text/plain; charset=utf-8
Content-Length: 2
Connection: keep-alive
X-Content-Type-Options: nosniff
ok
```

## RBAC for Kubelet Authorization

In this section you will configure RBAC permissions to allow the Kubernetes API Server to access the Kubelet API on each worker node. Access to the Kubelet API is required for retrieving metrics, logs, and executing commands in pods.

> This tutorial sets the Kubelet --authorization-mode flag to Webhook. Webhook mode uses the [Subject Access Review](https://kubernetes.io/docs/reference/access-authn-authz/authorization/#checking-api-access) API to determine authorization

Дальнейшие команды влияют на весь кластер, и их нужно запускать только один раз с одного из узлов контроллера
```sh
gcloud compute ssh controller-0
```
Создаем `system:kube-apiserver-to-kubelet` [Cluster Role](https://kubernetes.io/docs/reference/access-authn-authz/rbac/#role-and-clusterrole) с разрешениями для доступа к API Kubelet и выполнения наиболее распространенных задач, связанных с управлением подами 
```sh
cat <<EOF | kubectl apply --kubeconfig admin.kubeconfig -f -
apiVersion: rbac.authorization.k8s.io/v1beta1
kind: ClusterRole
metadata:
  annotations:
    rbac.authorization.kubernetes.io/autoupdate: "true"
  labels:
    kubernetes.io/bootstrapping: rbac-defaults
  name: system:kube-apiserver-to-kubelet
rules:
  - apiGroups:
      - ""
    resources:
      - nodes/proxy
      - nodes/stats
      - nodes/log
      - nodes/spec
      - nodes/metrics
    verbs:
      - "*"
EOF
```
Kubernetes API Server аутентифицируется в Kubelet как пользователь `kubernetes`, используя сертификат клиента, как определено флагом `--kubelet-client-certificate`  
Bind the `system:kube-apiserver-to-kubelet` ClusterRole to the `kubernetes` user
```sh
cat <<EOF | kubectl apply --kubeconfig admin.kubeconfig -f -
apiVersion: rbac.authorization.k8s.io/v1beta1
kind: ClusterRoleBinding
metadata:
  name: system:kube-apiserver
  namespace: ""
roleRef:
  apiGroup: rbac.authorization.k8s.io
  kind: ClusterRole
  name: system:kube-apiserver-to-kubelet
subjects:
  - apiGroup: rbac.authorization.k8s.io
    kind: User
    name: kubernetes
EOF
```

### The Kubernetes Frontend Load Balancer
In this section you will provision an external load balancer to front the Kubernetes API Servers. The `kubernetes-the-hard-way` static IP address will be attached to the resulting load balancer.

> The compute instances created in this tutorial will not have permission to complete this section. **Run the following commands from the same machine used to create the compute instances**

**`Provision a Network Load Balancer`**
- Create the external load balancer network resources
```sh
KUBERNETES_PUBLIC_ADDRESS=$(gcloud compute addresses describe kubernetes-the-hard-way \
  --region $(gcloud config get-value compute/region) \
  --format 'value(address)')

gcloud compute http-health-checks create kubernetes \
  --description "Kubernetes Health Check" \
  --host "kubernetes.default.svc.cluster.local" \
  --request-path "/healthz"

gcloud compute firewall-rules create kubernetes-the-hard-way-allow-health-check \
  --network kubernetes-the-hard-way \
  --source-ranges 209.85.152.0/22,209.85.204.0/22,35.191.0.0/16 \
  --allow tcp

gcloud compute target-pools create kubernetes-target-pool \
  --http-health-check kubernetes

gcloud compute target-pools add-instances kubernetes-target-pool \
  --instances controller-0,controller-1,controller-2

gcloud compute forwarding-rules create kubernetes-forwarding-rule \
  --address ${KUBERNETES_PUBLIC_ADDRESS} \
  --ports 6443 \
  --region $(gcloud config get-value compute/region) \
  --target-pool kubernetes-target-pool
```

**`Verification`**  
> The compute instances created in this tutorial will not have permission to complete this section. Run the following commands from the same machine used to create the compute instances.

- Получаем статик IP `kubernetes-the-hard-way`
```sh
KUBERNETES_PUBLIC_ADDRESS=$(gcloud compute addresses describe kubernetes-the-hard-way \
  --region $(gcloud config get-value compute/region) \
  --format 'value(address)')
```
- Курлом смотрим инфо о версии кубика в кластере
```sh
curl --cacert ca.pem https://${KUBERNETES_PUBLIC_ADDRESS}:6443/version

{
  "major": "1",
  "minor": "15",
  "gitVersion": "v1.15.3",
  "gitCommit": "2d3c76f9091b6bec110a5e63777c332469e0cba2",
  "gitTreeState": "clean",
  "buildDate": "2019-08-19T11:05:50Z",
  "goVersion": "go1.12.9",
  "compiler": "gc",
  "platform": "linux/amd64"
}
```

## Bootstrapping the Kubernetes Worker Nodes








## Доп. задание №1

## Доп. задание №2

[Вернуться к оглавлению ^](https://github.com/Otus-DevOps-2019-08/Lisskha_microservices#table-of-contents)

