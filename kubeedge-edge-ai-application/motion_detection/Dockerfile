FROM sixsq/opencv-python:master-arm
WORKDIR /code
COPY . /motion_detection
WORKDIR /motion_detection
RUN mkdir -p /motion_detection/data/video
RUN apt update
RUN apt install --assume-yes libgtk2.0-0 libnotify4
ENTRYPOINT ["python3","-u", "/motion_detection/detec_fram.py"]
