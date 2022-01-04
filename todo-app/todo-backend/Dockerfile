FROM node:16
USER node
WORKDIR /usr/src/app
COPY . .
RUN npm ci --production-only
ENV NODE_ENV=production
ENV MONGO_URL=mongodb://root:password@localhost:3456/development?authSource=admin&readPreference=primary&appname=MongoDB%20Compass&directConnection=true&ssl=false
CMD npm start