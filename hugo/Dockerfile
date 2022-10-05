FROM registry.gitlab.com/pages/hugo/hugo_extended:0:79.1

RUN apk add --update --nocache git

RUN apk add --update npm

ENTRYPOINT /user/bin/hugo
