FROM ubuntu:latest
EXPOSE 8888
RUN apt-get update && apt-get install -y iputils-ping
VOLUME /home/output
ENTRYPOINT ["ping", "www.facebook.pt"]
