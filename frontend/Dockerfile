FROM node:20-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

ENV REACT_APP_API_BASE_URL=${REACT_APP_API_BASE_URL}

CMD ["npm", "run", "dev", "--", "--host"]