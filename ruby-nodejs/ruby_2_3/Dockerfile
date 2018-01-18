FROM ruby:2.3.4

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash - \
  && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - \
  && echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list \
  && apt update && apt install --assume-yes nodejs yarn rsync \
  && rm -rf /var/lib/apt/lists/*
