FROM node:16.3.0-alpine

RUN mkdir -p /app
WORKDIR /app

COPY package.json package-lock.json ./

# install packages
RUN npm install -g @angular/cli
RUN npm install
RUN ng serve -o

COPY . /app 

EXPOSE 3000

CMD ["npm", "run", "start"]
