FROM alpine:latest

RUN apk add --no-cache dash git; \
git config --global user.email "user@example.com"; \
git config --global user.name "User Name";

COPY ../.. /opt/basher/

ENTRYPOINT ["/usr/bin/dash", "/opt/basher/bats/bin/bats"]
