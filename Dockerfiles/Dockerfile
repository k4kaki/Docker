FROM ubuntu
RUN apt-get update
RUN apt-get install vim -y
#CMD: Specifies the command to run when a container is launched, if values are specified during the launch it will override the Dockerfile value 
CMD ["echo","Sanjeeva"]
#ENTRYPOINT: This also same as CMD but unlike CMD whatever you give in arguments that will be appeneded along with ENTRYPOINT args.
ENTRYPOINT ["echo","Sanjeeva Kaki"]
#WORKDIR: whatever the path you give here it will go into that folder and execute the command
WORKDIR /tmp #we can overrite this by -w flag in args
RUN touch sanjeeva #creates sanjeeva file in /tmp folder
#ENV: is to set a environment variable 
#USER : will give default user name while logging in
#VOLUME : To create volume while invoking image / spinning the container
VOLUME ["/data"]
COPY DUMMYFILE /data/DUMMYFILE
ADD some.tar /data #will extract all the files and keep them inside the /data in the container
MAINTAINER SanjeevaKaki "myemail@gmail.com"
CMD ["/usr/sbin/apache2","-D","FOREGROUND"]
