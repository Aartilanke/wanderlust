FROM node:21
WORKDIR /app
COPY package*.json ./

# Install dependencies
RUN npm install

COPY . .
RUN npm i
COPY .env.sample .env.local
Expose 5173
CMD ["npm" , "run" , "dev" , "--" , "--host" ]
