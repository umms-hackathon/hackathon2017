**Docker**

Please install docker to your computer if you don't have

https://docs.docker.com/engine/installation/#desktop


To be able to run apache-mysql-php use wnameless/mysql-phpmyadmin 

```
docker pull wnameless/mysql-phpmyadmin
```

Run with 22, 80 and 3306 ports opened:

```
docker run -d -p 49160:22 -p 49161:80 -p 49162:3306 -v ~/Desktop:/srv wnameless/mysql-phpmyadmin
```

Open http://localhost:49161/phpmyadmin in your browser with following credential:

```
username: root
password:
```

**Login by SSH**

```
ssh root@localhost -p 49160
password: admin
```

