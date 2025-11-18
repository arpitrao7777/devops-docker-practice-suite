FROM node AS nod
WORKDIR /prod
COPY . .
RUN npm install
RUN npm run build

FROM nginx AS ng
COPY --from=nod /prod/build /usr/share
/nginx/html