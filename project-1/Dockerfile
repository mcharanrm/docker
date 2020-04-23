#Description: Build a image to run a container for infinite amount of time 

#Use alpine base image
FROM alpine:latest

#Update and Install bash interpreter
#RUN apk update && \
#   apk add bash && \ executing loop without using bash interpreter and minimizing size of image
#    mkdir /root/scripts && \
#    export PATH=$PATH:/root/scripts

#Copy scripts from local host to container
COPY . /root

#Startup script
ENTRYPOINT ["/bin/sh","/root/infinite_loop"]

