FROM python:2.7

WORKDIR /app

RUN git clone https://github.com/foosel/OctoPrint.git \
    && cd OctoPrint \
    && virtualenv venv \
    && ./venv/bin/pip install . \
    && ./venv/bin/octoprint serve
