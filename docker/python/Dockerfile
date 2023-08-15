FROM python:3.7
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install \
    gcc nano \
    ffmpeg libasound-dev portaudio19-dev libportaudio2 libportaudiocpp0 alsa-utils usbutils \
    postgresql postgresql-contrib -y
RUN pip install numpy scipy matplotlib pydub pyaudio psycopg2

COPY ./onsite_node/dejavu-stx ./code
WORKDIR /code