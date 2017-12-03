# codeblick/lamp

## About

This images contains a LAMP stack (Apache + MySQL + PHP). It is based on [our php image](https://hub.docker.com/r/codeblick/php/).

## Usage

```shell
docker run \
	-p 80:80 \
	-p 3306:3306 \
	-e "MYSQL_ROOT_PASSWORD=rootpwd" \
	-e "MYSQL_DATABASE=dbname" \
	-e "MYSQL_USER=dbuser" \
	-e "MYSQL_PASSWORD=dbpwd" \
	-v $PWD:/var/www/html \
	codeblick/lamp:7.1-apache-mysql
```

