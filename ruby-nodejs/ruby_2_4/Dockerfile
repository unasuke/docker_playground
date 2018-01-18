FROM ruby:2.4.2

RUN curl -sL https://deb.nodesource.com/setup_8.x | bash - \
  && apt update && apt install --assume-yes nodejs \
  && rm -rf /var/lib/apt/lists/*
