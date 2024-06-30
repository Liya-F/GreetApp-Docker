# Use a lightweight web server image to serve static content
FROM nginx:alpine

# Copy the content of the frontend folder to the default Nginx public folder
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80 to the outside world
EXPOSE 80

# CMD to start Nginx and keep the process from backgrounding and container to exit.
CMD ["nginx", "-g", "daemon off;"]
