FROM ubuntu

#!/bin/bash

WORKDIR /ws_events

COPY config.yml /ws_events/config.yml
COPY ws_events /ws_events/ws_events
COPY main.html /ws_events/main.html
COPY main_guest.html /ws_events/main_guest.html
COPY user_events.html /ws_events/user_events.html

RUN chmod +x /ws_events

CMD ["./ws_events/ws_events"]