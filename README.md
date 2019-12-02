# Build Status
![Build Status](https://travis-ci.com/anthonyptetlow/docker-composer.svg?branch=master)

# Usage
```
docker run -it --rm -u $( id -u $user ):$( id -g $user ) -v /etc/group:/etc/group:ro -v /etc/passwd:/etc/passwd:ro -v ~/.composer:/composer -v ~/.ssh:/home/${USER}/.ssh -v ${PWD}:/app -w /app thedrum/composer update
```
