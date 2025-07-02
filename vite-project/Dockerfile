FROM nginx:alpine

# Copy the built app from the previous stage
COPY dist /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]