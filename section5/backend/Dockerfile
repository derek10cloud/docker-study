FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=derek
ENV MONGODB_PASSWORD=secret

CMD ["npm", "start"]
