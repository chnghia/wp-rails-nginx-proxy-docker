FROM ruby:2.4
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /var/www/webapp
WORKDIR /var/www/webapp
COPY rails/Gemfile /var/www/webapp/Gemfile
COPY rails/Gemfile.lock /var/www/Gemfile.lock
RUN bundle install
COPY rails /var/www/webapp