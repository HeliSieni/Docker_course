
FROM golang:1.16

EXPOSE 8080
#for the exc1.14
ENV REQUEST_ORIGIN=http://localhost:5000
COPY . /usr/src/app
WORKDIR /usr/src/app/example-backend
RUN go build
CMD ./server
