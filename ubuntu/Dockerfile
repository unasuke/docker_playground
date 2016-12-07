FROM ubuntu:xenial

# set timezone to Asia/Tokyo (JST)
RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime

# dependency
RUN apt update \
    && apt install -y \
          autoconf        \
          bison           \
          bzip2           \
          cgroup-bin      \
          curl            \
          flex            \
          git-core        \
          g++             \
          libcgroup-dev   \
          libpam0g-dev    \
          libreadline-dev \
          libssl-dev      \
          libtool         \
          make            \
          ruby            \
          vim-nox         \
          wget            \
          zlib1g-dev

# rbenv
RUN git clone https://github.com/rbenv/rbenv.git ~/.rbenv \
    && echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc \
    && git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build \
    && source ~/.bashrc \
    && rbenv install 2.3.3 \
    && rbenv global 2.3.3


RUN git clone https://github.com/haconiwa/haconiwa.git ~/src/github.com/haconiwa/haconiwa
