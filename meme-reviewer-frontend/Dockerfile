FROM node:16.14.0-alpine

WORKDIR /app

COPY package.json .
COPY package-lock.json .
RUN npm install

COPY . .

EXPOSE 3000
ENTRYPOINT ["npm", "start"]

# check if you are in the correct folder -> cd meme-reviewer-frontend

# build the image -> docker build -t mr-frontend:latest .

# run the container -> docker run -p 5000:5000 mr-frontend:latest