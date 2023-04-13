# FROM ubuntu

# RUN apt update
# RUN apt install curl --yes
# RUN apt install vim --yes
# RUN apt install git --yes

# # outra opção para instalar os pacotes de cima é:
# # RUN apt update && apt install curl vim git --yes

FROM node:18.11.0

WORKDIR /app
COPY package*.json ./
RUN npm install 
COPY . . 
EXPOSE 8080
CMD [ "node", "server.js" ]
