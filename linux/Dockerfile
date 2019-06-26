FROM openjdk:8-jre

RUN apt-get update && apt-get install -y --no-install-recommends \
        git  \
        curl \
        nano \
        htop \
		xvfb \
		libxext6
		
ENV DISPLAY=:99
ENV DISPLAY_CONFIGURATION=1024x768x24

ARG workdir=/workspace
ARG bin=cli-linux-x64

WORKDIR $workdir

COPY $bin $workdir/katalon-agent
