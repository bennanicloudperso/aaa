FROM node:20 AS build-env
COPY . /app
WORKDIR /app
RUN npm i


FROM gcr.io/distroless/nodejs20-debian11
COPY --from=build-env /app /app
WORKDIR /app
EXPOSE 3000

CMD ["server.js"]