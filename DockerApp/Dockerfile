# Simple Dockerfile: serve the current directory over HTTP on port 8000
FROM  ubuntu

WORKDIR /home/anchor/WorkSpace/DevOps/DockerApp/

RUN  apt-get update &&  \
     apt-get install -yq build-essential make git libsqlite3-dev sqlite3

COPY . /opt/

WORKDIR /opt/facebooc

RUN make all

EXPOSE 16000


CMD ["bin/facebooc"]

