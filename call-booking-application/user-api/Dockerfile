FROM node:17.9.0-slim
LABEL maintainer="Anil Nalawade"

RUN useradd userapi
WORKDIR /app
COPY . . 
RUN npm install
EXPOSE 1004
USER userapi
ENV MONGO_URL=""
ENV ADMIN_EMAIL=""
ENTRYPOINT [ "npm", "start" ]