FROM node:14
WORKDIR /app
RUN mkdir tmp
RUN mkdir assets
COPY ./package*.json /app/
RUN npm install
COPY *.js /app/
COPY assets/* /app/assets
COPY tmp /app/
CMD ["node","/app"]
