# Running MariaDB in a Docker container.
![Docker & MariaDB banner](/images/docker-mariadb-banner.png)

### Docker automated builds
The Docker automated builds can be found over here: https://hub.docker.com/r/containerstack/docker-mariadb

### Pull Docker image
docker pull remonlam/docker-mariadb

### Start a container based on this image
docker run --detach \ <br>
  --publish [port:port] \ <br>
  --name [name] \ <br>
  --volume [path] \ <br>
  --link mysql:mysql \ <br>
  --env [env1=something] \ <br>
    containerstack/docker-mariadb
