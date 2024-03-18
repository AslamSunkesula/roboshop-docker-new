FROM debian:latest 
RUN apt-get update && apt-get install -y nginx
RUN rm -rf /usr/share/nginx/html/index.html
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf
ADD static /usr/share/nginx/html/
