FROM centos

# Install sudo and nginx
RUN yum -y install epel-release && \
    yum -y install sudo nginx && \
    yum clean all

# Remove default nginx configuration
RUN rm -f /etc/nginx/nginx.conf \
    && rm -f /etc/nginx/conf.d/default.conf

# Copy custom nginx configuration
COPY roboshop.conf /etc/nginx/nginx.conf

# Copy static files to nginx HTML directory
COPY static /usr/share/nginx/html/

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]
