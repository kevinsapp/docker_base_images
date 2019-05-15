# This Dockerfile is used to build and run a Ruby on Rails
# environment inside a container.
FROM ruby:2.6.3-stretch

# Install apt based dependencies required to run Rails and RubyGems.
# Rails requires a JavaScript runtime, so install Node.js too.
RUN apt-get update \
    && apt-get install -y \
        postgresql-client \
        build-essential \
        nodejs \
    && rm -rf /var/lib/apt/lists/*

# Install Rails
RUN gem install rails -v 5.2.3
