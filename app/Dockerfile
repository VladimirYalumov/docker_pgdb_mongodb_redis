FROM amazonlinux

#!/bin/sh

WORKDIR /app

COPY config.yml /app/config.yml

# restapi
COPY restapi /app/restapi
COPY errors.json /app/errors.json

# events
COPY events /app/events

# консьюмеры для обработки запросов на поиск
COPY search_main /app/search_main
COPY search_user /app/search_user

# вебсокеты + демо страницы, которых не будет на проде
COPY ws_events /app/ws_events
COPY main.html /app/main.html
COPY main_guest.html /app/main_guest.html
COPY user_events.html /app/user_events.html

COPY database /app/database

CMD ["./search_user &"]
CMD ["./search_main &"]
CMD ["./events &"]
CMD ["./restapi &"]
CMD ["./ws_events &"]

# миграции созание всех таблиц и партиций на этот год. Также есть стартовые данные.
CMD ["./database"]