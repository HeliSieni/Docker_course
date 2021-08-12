# Start ubuntu
FROM ubuntu:18.04

#copy the script
COPY skripti.sh . 

#curl is needed
RUN apt-get update; apt-get install -y curl

# Let's give the command "server"
CMD  ./skripti.sh
