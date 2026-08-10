FROM ubuntu:24.04

RUN apt-get update
RUN apt-get install -y git curl wget build-essential ruby-full zlib1g-dev

RUN gem install bundler --no-document

RUN wget https://raw.githubusercontent.com/Radon10043/Radon10043.github.io/refs/heads/master/Gemfile && \
    wget https://raw.githubusercontent.com/Radon10043/Radon10043.github.io/refs/heads/master/Gemfile.lock && \
    bundle install && \
    rm Gemfile Gemfile.lock

RUN git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && \
    ~/.fzf/install
