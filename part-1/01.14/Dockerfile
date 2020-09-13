FROM ruby:2.6.0

RUN gem install bundler
RUN bundle install
RUN rails db:migrate

CMD ["rails","s"]
