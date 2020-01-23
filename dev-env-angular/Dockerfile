FROM node:latest

ENV APPLICATION_ROOT /application

RUN mkdir $APPLICATION_ROOT
WORKDIR $APPLICATION_ROOT
VOLUME $APPLICATION_ROOT # TODO: ホストにマウント出来ていなさそう

RUN apt update && \
    apt upgrade && \
    npm install -g @angular/cli && \
    apt autoremove && \
    apt autoclean

EXPOSE 80 # TODO: ホストにポート割当出来ていない（READMEのコマンドも見直す）
