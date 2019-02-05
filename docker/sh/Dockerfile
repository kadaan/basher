ARG shell=sh

FROM alpine:latest

RUN apk add --no-cache git; \
git config --global user.email "user@example.com"; \
git config --global user.name "User Name";

COPY . /opt/basher/

ENTRYPOINT ["/bin/${shell}", "/opt/basher/bats/bin/bats"]
