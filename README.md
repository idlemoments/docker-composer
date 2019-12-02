# Supported tags and respective `Dockerfile` links
 - 7.4, latest (*[7.4/Dockerfile](./7.4/Dockerfile)*)
 - 7.3, latest (*[7.3/Dockerfile](./7.3/Dockerfile)*)
 - 7.2, latest (*[7.2/Dockerfile](./7.2/Dockerfile)*)
 - 7.1, latest (*[7.1/Dockerfile](./7.1/Dockerfile)*)
 - 7.0, latest (*[7.0/Dockerfile](./7.0/Dockerfile)*)

# Usage
```
docker run -it --rm -u $( id -u $user ):$( id -g $user ) -v /etc/group:/etc/group:ro -v /etc/passwd:/etc/passwd:ro -v ~/.composer:/composer -v ~/.ssh:/home/${USER}/.ssh -v ${PWD}:/app -w /app thedrum/composer update
```
