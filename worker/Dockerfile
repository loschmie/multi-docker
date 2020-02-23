FROM node:alpine
WORKDIR /app
COPY package.json .
RUN npm install && npm audit fix --force
RUN npm fund
COPY . .
CMD [ "npm", "run", "start" ]