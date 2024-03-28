FROM node:14-alpine

WORKDIR /app

ENTRYPOINT [ "npm" ]

# docker run -it -v /home/danio/personal/wa/docker-course/first-utility-container:/app node-util npm init with this command we launch the npm init. But now we have created an utility container thanks to the bind mount that reflect out to our host machine, so we can uninstall node and npm and continue to use them thanks to this utility container

# if we insert a command after docker run and the container name like this docker run -it -v /home/danio/personal/wa/docker-course/first-utility-container:/app node-util npm init we overwrite the CMD into the docker file if there is one, to avoid this, use the ENTRYPOINT, that allow us to APPEND the command we insert after the container name, to the entrypoint commands. So, now we don't use npm init, but only init: docker run -it -v /home/danio/personal/wa/docker-course/first-utility-container:/app mynpm init
# This is possible thanks to the bind mount