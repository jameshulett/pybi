FROM continuumio/anaconda

# Install our python requirements
COPY requirements.txt /tmp
RUN pip install -r /tmp/requirements.txt

RUN mkdir -p /home/shared/rodeo

CMD ["rodeo", "/home/shared/rodeo", "--host=0.0.0.0", "--no-browser"]
