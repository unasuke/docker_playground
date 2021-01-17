FROM rubylang/ruby:3.0-focal
RUN apt update && apt install --assume-yes --no-install-recommends curl gpg-agent \
  && curl -sL https://deb.nodesource.com/setup_14.x | bash - \
  && apt update && apt install --assume-yes --no-install-recommends nodejs \
  && rm -rf /var/lib/apt/lists/*
