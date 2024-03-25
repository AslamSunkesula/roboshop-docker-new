FROM almalinux:latest
RUN yum install -y nginx
RUN rm -rf /usr/share/nginx/html/index.html
#COPY roboshop.conf /etc/nginx/nginx.conf
CMD ["nginx", "-g", "daemon off;"] 