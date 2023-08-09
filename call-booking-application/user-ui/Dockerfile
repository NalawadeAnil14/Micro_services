FROM node:17.9.0-slim
LABEL maintainer="Anil Nalawade"

RUN useradd userui 
WORKDIR /app
COPY . . 
RUN npm install
EXPOSE 3000
USER userui
ENTRYPOINT [ "npm", "start" ]