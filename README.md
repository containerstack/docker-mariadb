# MariaDB in Docker container

### Repo info
This repo will build a MariaDB inside a Docker container.<br>
It used the original Dockerfile provided by the MariaDB project team, however for OS X users I have added a extra Dockerfile (located in /osx/Dockerfile) that build one that make mounts working on OS X.

### Mount volumes from the Docker host on OSX
When you're running Docker on OSX with help of the Docker Toolbox, and when you want to use the "--volume" option to mount a directory from the host to the container, you will end up with a permission error when the application that's running inside the container uses an other account than root to run the app
