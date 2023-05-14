FROM ubuntu

#!/bin/bash

WORKDIR /ws_events

COPY config.yml /ws_events/config.yml
COPY web_socket /ws_events/web_socket

RUN chmod +x /ws_events

CMD ["./ws_events/web_socket"]