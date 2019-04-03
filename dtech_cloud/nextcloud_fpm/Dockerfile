FROM nextcloud:fpm-alpine

RUN set -ex; \
    \
    apk add --no-cache \
        ffmpeg \
        imagemagick \
        samba-client \
        supervisor \
      libreoffice \
    ;

ENV NEXTCLOUD_UPDATE=1