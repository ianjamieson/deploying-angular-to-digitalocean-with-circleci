FROM nginx:1.17.5-alpine

## Copy our default nginx config
COPY nginx/staging-default.conf /etc/nginx/conf.d/default.conf

## Remove default nginx website
RUN rm -rf /usr/share/nginx/html/*

## Assumes you've built the app in the current working directory
COPY dist /usr/share/nginx/html

CMD ["nginx", "-g", "daemon off;"]
