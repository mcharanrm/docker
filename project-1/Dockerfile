#Description: Build a image to run a container for infinite amount of time 

#Use alpine base image
FROM alpine:latest

#Update and Install bash interpreter
RUN apk update && \
    apk add bash && \
    mkdir /root/scripts && \
    export PATH=$PATH:/root/scripts

#Copy scripts from local host to container
COPY . /root/scripts/

#Startup script
ENTRYPOINT ["/root/scripts/loop.sh",">","/dev/null"]

