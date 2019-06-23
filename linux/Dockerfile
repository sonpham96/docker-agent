FROM openjdk:8-jre

RUN apt-get update && apt-get install -y --no-install-recommends \
        git  \
        curl \
        nano \
        htop

ARG workdir=/workspace
ARG bin=cli-linux-x64

WORKDIR $workdir

COPY $bin $workdir/katalon-agent
