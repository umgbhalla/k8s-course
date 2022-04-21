FROM node:14
RUN mkdir -p /app && chown -R node:node /app
WORKDIR /app
USER node
RUN mkdir tmp
RUN mkdir assets
COPY --chown=node ./package*.json /app/
RUN npm install
COPY --chown=node *.js /app/
COPY --chown=node assets/* /app/assets
COPY --chown=node tmp /app/
CMD ["node","/app"]
