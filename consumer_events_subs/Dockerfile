FROM ubuntu

#!/bin/bash

WORKDIR /consumer_events_subs

COPY config.yml /consumer_events_subs/config.yml
COPY subs_consumer /consumer_events_subs/subs_consumer

RUN chmod +x /consumer_events_subs

CMD ["./consumer_events_subs/subs_consumer"]