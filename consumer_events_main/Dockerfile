FROM ubuntu

#!/bin/bash

WORKDIR /consumer_events_main

COPY config.yml /consumer_events_main/config.yml
COPY search_main /consumer_events_main/search_main

RUN chmod +x /consumer_events_main

CMD ["./consumer_events_main/restapi"]