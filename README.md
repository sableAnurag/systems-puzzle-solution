# Insight DevOps Engineering Systems Puzzle

## Changes made:


# docker-compose.yml

Order of ports specified for Nginx server was reversed, it should be "host_port":container_port", not reverse.

# app.py

Flask app connection issue with DB Server (Postgres), does not always connect correctly(best guess, docker-compose does not wait for db ready) , also, port for app to connect to DB was not mentioned, observed from error log of DB service.

Also, after fix, no more need for bootstrapping the database.


## System Config:

Debug, Run and Tested on Mac.

## PS

This puzzle was fun!




