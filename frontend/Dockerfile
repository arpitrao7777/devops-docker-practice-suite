FROM node
WORKDIR /dev
COPY . .
RUN npm install
RUN npm run build

RUN apt update
RUN apt install nginx -y
RUN cp -r build/* /var/www/html
ENTRYPOINT nginx -g 'daemon off;'