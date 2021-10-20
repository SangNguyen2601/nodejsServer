# Dockerfile  
FROM node:12.16.1
#RUN mkdir -p /usr/src/app/server
WORKDIR /usr/src/app/server
COPY ./package.json ./
RUN npm install
RUN npm audit fix
COPY ./ ./
EXPOSE 3100
    
CMD ["npm", "start"]