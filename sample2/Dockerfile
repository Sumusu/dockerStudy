FROM ubuntu:latest

RUN apt-get update && apt-get install -y cowsay fortune
ADD entrypoint.sh /
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
