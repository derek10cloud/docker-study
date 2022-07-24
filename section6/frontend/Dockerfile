FROM node

WORKDIR /app

COPY package.json .

RUN npm install --save react-scripts@5.0.1

COPY . .

EXPOSE 3000

CMD [ "npm", "start" ]
