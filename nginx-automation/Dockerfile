 # What will the base image be?
 FROM nginx

 # What do you want in the image
 COPY index.html /usr/share/nginx/html

 # What ports the image will need to be able to use?
 EXPOSE 80

 # Launch the server itself
 CMD ["nginx", "-g", "daemon off;"]
