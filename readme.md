this is an simple react app for development environment wherein the cahnges get refelcted inside the container


```
 docker build -t "react-app-1" -f Dockerfile.dev .  # this will build the image and tag the image with name :react-app-1;
 docker run -p 3000:3000 -v /usr/app/node_modules -v $(pwd):/usr/app react-app-1    
 #  -v /usr/app/node_modules is bookmark of volume 
 #  -v $(pwd):/usr/app is used mount [local drive volume]: [container volume] 
```