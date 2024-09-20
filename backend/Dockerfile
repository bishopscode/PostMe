FROM node:latest
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
ARG JWT_SECRET
ENV JWT_SECRET=$JWT_SECRET
CMD ["npm", "start"]