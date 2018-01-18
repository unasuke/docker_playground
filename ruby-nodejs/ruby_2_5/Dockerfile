FROM ruby:2.5.0

RUN curl -sL https://deb.nodesource.com/setup_9.x | bash - \
  && apt update && apt install --assume-yes nodejs \
  && rm -rf /var/lib/apt/lists/*
