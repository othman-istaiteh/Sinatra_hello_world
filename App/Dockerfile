FROM ruby:3.0.2

WORKDIR /usr/src/app

COPY Gemfile ./
RUN bundle install

EXPOSE 4567

COPY . .

CMD ["bundle", "exec", "rackup", "--host", "0.0.0.0", "-p", "4567"]