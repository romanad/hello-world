# Use the official Nginx image as the base image
FROM nginx:latest

# Optional: Set the maintainer label
LABEL maintainer="adroman@yandex.ru"

# Set working directory to nginx asset directory
#WORKDIR /usr/share/nginx/html

# Remove the default nginx static assets
# RUN rm -rf ./*

# Copy a new configuration file (if you have)
# COPY nginx.conf /etc/nginx/nginx.conf

# Copy static assets over
#COPY static-html-directory/ .

# Expose port 80 to the outside once the container has launched
EXPOSE 80

# Define the command to run your app using CMD which defines your runtime
# Here we use the "daemon off;" command to run Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
