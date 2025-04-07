FROM alpine:3.16

# Instala Python3 y pip3
RUN apk add --no-cache python3 py3-pip

ADD requirements.pip requirements.pip
RUN pip3 install -r requirements.pip

ADD src src

EXPOSE 5000

CMD ["python3", "/src/run.py"]
