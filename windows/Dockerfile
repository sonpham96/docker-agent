FROM openjdk:8-jre-windowsservercore-1809

RUN net user /add agent
RUN net localgroup Administrators agent /add
USER agent

ENV USERPROFILE="C:\Users\agent"

ARG workdir=/workspace
ARG bin=cli-win-x64.exe

WORKDIR $workdir

COPY $bin $workdir/katalon-agent.exe
