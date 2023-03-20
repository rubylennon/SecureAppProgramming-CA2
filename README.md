# Main

Command to create a docker network called 'my-network'
```
docker network create my-network
```

Command to run a mysql:latest docker image with the name of 'db' with a root password of 'my-secret-password'
```
docker run --name db -e MYSQL_ROOT_PASSWORD=my-secret-password -d mysql:latest
```

Command to run docker image phpmyadmin/phpmyadmin on network 'my-network' and map port 8080 to port 80  the container
```
docker run --network my-network -p 8080:80 phpmyadmin/phpmyadmin
```
