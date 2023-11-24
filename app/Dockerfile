FROM alpine:latest
RUN apk add go git
WORKDIR /src
ADD . .
RUN go build
EXPOSE 80
CMD [ "/bin/sh", "-c", "/src/app http://db > /var/log/tns-app.log" ]
