FROM klakegg/hugo:ext-alpine

RUN apk add git && \
  git config --global --add safe.directory /src
  
RUN npm install
RUN npm install -g @fullhuman/postcss-purgecss rtlcss
