FROM amazonlinux:2

# Install Nginx.
RUN amazon-linux-extras install -y nginx1.12

# Run Nginx
CMD ["nginx", "-g", "daemon off;"]

COPY default.conf /etc/nginx/conf.d/
COPY index.html /usr/share/nginx/html/

# Expose ports.
EXPOSE 80
EXPOSE 443