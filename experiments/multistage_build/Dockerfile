FROM node:14-alpine as builder

WORKDIR /app
COPY ./secret.txt /app/secret.txt
RUN touch runnable

FROM node:14-alpine

WORKDIR /app
COPY --from=builder /app/runnable .
