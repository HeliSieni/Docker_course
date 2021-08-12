# Let's use ubuntu as nothing special was needed
FROM ubuntu:18.04

EXPOSE 5000
COPY . /usr/src/app
WORKDIR /usr/src/app/example-frontend

#for exc1.14
#ENV REACT_APP_BACKEND_URL=http://localhost:8080

#curl is needed
RUN apt-get update; apt-get install -y curl


# From README
RUN  curl -sL https://deb.nodesource.com/setup_14.x | bash
RUN  apt install -y nodejs
RUN npm install
RUN npm run build
RUN npm install -g serve

#add the -n option to get rid of the xsel error
CMD ["serve", "-n", "-s" ,"-l", "5000", "build"]
