FROM node:16.14.2

ADD dist /app
COPY node_modules /app/node_modules
COPY main.js /app/main.js
COPY package.json /app/package.json

EXPOSE 3000
CMD ["node", "/app/main.js"]
