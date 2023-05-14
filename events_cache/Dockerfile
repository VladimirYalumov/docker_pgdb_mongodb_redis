FROM ubuntu

#!/bin/bash

WORKDIR /events_cache

COPY config.yml /events_cache/config.yml
COPY events_cache /events_cache/events_cache

RUN chmod +x /events_cache

CMD ["./events_cache/events_cache"]