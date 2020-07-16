FROM ruby:2.6.0

RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt-get install -y nodejs

WORKDIR /myapp

COPY ./rails-example-project .

RUN gem install bundler

RUN bundle install

ENV RAILS_ENV=production

ENV SECRET_KEY_BASE=productionsecretkey

ENV RAILS_LOG_TO_STDOUT=true

RUN rails db:migrate

RUN rake assets:precompile

CMD rails s -e production
