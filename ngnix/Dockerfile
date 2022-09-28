FROM nginx:alpine
COPY ./ngnix/ngnix.conf /etc/nginx/conf.d/configfile.template
COPY ./example/public/index.xml /usr/share/nginx/html/index.xml

ENV PORT 8080
ENV HOST 0.0.0.0
EXPOSE 8080
CMD sh -c "envsubst '\$PORT' < /etc/nginx/conf.d/configfile.template > /etc/nginx/conf.d/default.conf && nginx -g 'daemon off;'"
