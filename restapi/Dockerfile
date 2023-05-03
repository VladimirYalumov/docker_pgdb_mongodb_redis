FROM ubuntu

#!/bin/bash

WORKDIR /restapi

COPY config.yml /restapi/config.yml
COPY restapi /restapi/restapi
COPY database /restapi/database
COPY errors.json /restapi/errors.json

RUN chmod +x /restapi

CMD ["./restapi/restapi"]