FROM centos:7

RUN yum install -y \
        automake        \
        autoconf        \
        bison           \
        bzip2           \
        flex            \
        gcc             \
        gcc-c++         \
        git-core        \
        glibc-static    \
        libtool         \
        make            \
        openssl-devel   \
        pam-devel       \
        readline-devel  \
        zlib-devel

# rbenv
RUN git clone https://github.com/rbenv/rbenv.git ~/.rbenv \
    && echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc \
    && echo 'eval "$(rbenv init -)"' >> ~/.bashrc \
    && git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build \
    && source ~/.bashrc \
    && rbenv install 2.3.3 \


RUN git clone https://github.com/haconiwa/haconiwa.git ~/src/github.com/haconiwa/haconiwa \
    && cd ~/src/github.com/haconiwa/haconiwa \
    && rbenv global 2.3.3 \
    && rake compile
