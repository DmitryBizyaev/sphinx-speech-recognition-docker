FROM ubuntu:20.04

RUN apt-get update && \
    apt-get install -y git python3-pip && \
    pip3 install --upgrade pip && \
    pip3 install Flask && \
    git clone https://github.com/DmitryBizyaev/sphinx-speech-recognition-manual-frontend.git && \
    cd sphinx-speech-recognition-manual-frontend

WORKDIR /sphinx-speech-recognition-manual-frontend

CMD [ "flask", "run", "--host=0.0.0.0", "--port=5555" ]

EXPOSE 5555