FROM almalinux:latest
RUN yum install -y nginx
RUN rm -rf /usr/share/nginx/html/index.html
ADD static /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"#]