FROM python:2.7

RUN useradd -ms /bin/bash pi

USER pi

WORKDIR /home/pi

RUN git clone https://github.com/foosel/OctoPrint.git \
    && cd OctoPrint \
    && virtualenv venv \
    && ./venv/bin/pip install . 

ENV PATH "$PATH:/home/pi/OctoPrint/venv/bin"

ENTRYPOINT 'octoprint' 
CMD 'serve'
