FROM nginx
RUN rm -rf /usr/share/nginx/html/index.html
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf
ADD static /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]