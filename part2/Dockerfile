# Use an official Nginx runtime as the base image
FROM nginx:latest

# Copy the HTML, CSS, and other files into the Nginx document root
COPY styles.css /usr/share/nginx/html/
COPY surveyform.html /usr/share/nginx/html/

# Set the working directory to the Nginx document root
WORKDIR /usr/share/nginx/html

# Expose port 80 for serving the web application
EXPOSE 80

# Start Nginx when the container runs
CMD ["nginx", "-g", "daemon off;"]





