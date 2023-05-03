FROM ubuntu

#!/bin/bash

WORKDIR /consumer_events_user

COPY config.yml /consumer_events_user/config.yml
COPY search_user /consumer_events_user/search_user

RUN chmod +x /consumer_events_user

CMD ["./consumer_events_user/search_user"]