FROM ubuntu:20.04

WORKDIR /app

RUN apt-get update && \
    apt-get install -y git python3-pip && \
    git clone https://github.com/DmitryBizyaev/sphinx-speech-recognition-manual.git && \
    cd /sphinx-speech-recognition-manual

CMD [ "python3", "request_handler.py" ]
EXPOSE 5555