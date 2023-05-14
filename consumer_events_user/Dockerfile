FROM ubuntu

#!/bin/bash

WORKDIR /consumer_events_user

COPY config.yml /consumer_events_user/config.yml
COPY user_consumer /consumer_events_user/user_consumer

RUN chmod +x /consumer_events_user

CMD ["./consumer_events_user/user_consumer"]