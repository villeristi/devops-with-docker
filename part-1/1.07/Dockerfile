FROM ubuntu:16.04
RUN apt-get update && apt-get install -y curl

WORKDIR /app
COPY curler.sh .
RUN chmod +x curler.sh

CMD ["./curler.sh"]
