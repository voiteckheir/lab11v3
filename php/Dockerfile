FROM php:fpm-alpine as php

#WORKDIR /usr/src/myapp

RUN apk update && apk add --no-cache \
    curl \
    && rm -rf /var/cache/apk/*

EXPOSE 9000

HEALTHCHECK --interval=30s --timeout=30s --start-period=5s --retries=3 \
    CMD  ["curl localhost:9000"]

CMD ["php-fpm" ]
#CMD ["start"]

# CMD [ "php", "./index.php" ] 