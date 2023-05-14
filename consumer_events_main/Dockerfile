FROM ubuntu

#!/bin/bash

WORKDIR /consumer_events_main

COPY config.yml /consumer_events_main/config.yml
COPY main_consumer /consumer_events_main/main_consumer

RUN chmod +x /consumer_events_main

CMD ["./consumer_events_main/main_consumer"]