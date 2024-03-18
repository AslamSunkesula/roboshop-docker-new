# Use the Ubuntu base image
FROM ubuntu:latest

# Update package lists and install NGINX
RUN apt update && apt install -y nginx 

# Remove the default NGINX landing page
RUN rm -rf /usr/share/nginx/html/index.html

# Copy custom NGINX configuration file
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf

# Add static files to NGINX web root directory
ADD static /usr/share/nginx/html/

# Expose port 80 (the default port used by NGINX)
EXPOSE 80

# Command to start NGINX when the container starts
CMD ["nginx", "-g", "daemon off;"]
