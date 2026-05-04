FROM nginx:1.27-alpine

RUN apk add --no-cache tzdata \
    && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo "Asia/Shanghai" > /etc/timezone

COPY default.conf /etc/nginx/conf.d/default.conf
EXPOSE 80 443
