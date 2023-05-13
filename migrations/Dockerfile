FROM ubuntu

#!/bin/bash

WORKDIR /migrations

COPY config.yml /migrations/config.yml
COPY database /migrations/database

RUN chmod +x /migrations

CMD ["./migrations/database"]