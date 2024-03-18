FROM nginx:1.24.0
RUN rm -rf /usr/share/nginx/html/index.html
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf
ADD static  /usr/share/nginx/html/