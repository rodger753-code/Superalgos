FROM node:15-alpine
WORKDIR /opt/superalgos
COPY . .
RUN adduser --disabled-password --no-create-home superalgos
RUN chown -R superalgos:superalgos /opt/superalgos
USER superalgos
EXPOSE 34248
EXPOSE 18041
ENTRYPOINT ["node", "run", "noBrowser"]
