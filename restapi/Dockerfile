FROM amazonlinux

#!/bin/sh

WORKDIR /app

COPY deewave_restapi /app/deewave_restapi
COPY config.yml /app/config.yml
COPY errors.json /app/errors.json

ENTRYPOINT ["./deewave_restapi"]