FROM node:20-alpine
WORKDIR /home/project
COPY ./package.json .
RUN yarn
COPY . .
RUN yarn global add vite
CMD ["yarn","dev"]