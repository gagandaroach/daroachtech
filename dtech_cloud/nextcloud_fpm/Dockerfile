FROM nextcloud:fpm-alpine

RUN set -ex; \
    \
    apk add --no-cache \
        # ffmpeg \
        imagemagick \
        # samba-client \
      libreoffice \
    ;

ENV NEXTCLOUD_UPDATE=1