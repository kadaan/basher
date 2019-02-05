FROM alpine:latest

RUN apk add --no-cache zsh git; \
git config --global user.email "user@example.com"; \
git config --global user.name "User Name";

COPY ../.. /opt/basher/

ENTRYPOINT ["/bin/zsh", "/opt/basher/bats/bin/bats"]
