FROM ubuntu

#!/bin/bash

WORKDIR /events_cache

COPY config.yml /events_cache/config.yml
COPY events /events_cache/events

RUN chmod +x /events_cache

CMD ["./events_cache/events"]