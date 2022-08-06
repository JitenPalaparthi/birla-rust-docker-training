FROM ubuntu

RUN apt-get update && \
apt-get upgrade -y && \
apt-get install vim -y

# To create a directory and make it as the work directory
WORKDIR /home/commands 

# Copy a file from source to destination.
# Here source is relative path,so all files and if directories from where this Dockerfile is there
# destination is . that means from the above command it is /home/commands directory
COPY * .

#RUN apt-get upgrade -y

#RUN apt-get install vim -y

CMD [ "bash" ]

# Run container
# exec container
# run apt-get update
# run apt-get upgrade 
# ru apt-get install vim





