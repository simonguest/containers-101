FROM ruby:2.7

# apt update and required libs
RUN apt-get update && apt-get install -y nodejs npm --no-install-recommends

# Install MySQL Native Client
RUN apt-get -y install mariadb-client-core-10.5

# Install rails and bundler
RUN ["gem", "install", "rails", "bundler"]

# Install yarn
RUN ["npm","i","-g","yarn"]

# Bundle install
COPY /app/Gemfile /app/Gemfile.lock ./
RUN bundle install

EXPOSE 3000

WORKDIR /opt/app