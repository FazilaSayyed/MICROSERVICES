FROM ubuntu:latest
LABEL microservices="counter"
RUN apt update
RUN apt install nginx -y
RUN rm -rf /var/www/html/index.html
WORKDIR /var/www/html/
COPY counter/* .
EXPOSE 80
CMD ["nginx", "-g","daemon off;"] 