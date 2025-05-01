# Use the official Nginx base image
FROM nginx:alpine

# Copy your HTML files into the default Nginx directory
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]