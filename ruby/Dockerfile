FROM ruby:3.4.2

WORKDIR /opt/app
COPY . .
WORKDIR /opt/app/ruby

RUN bundle update --bundler
RUN bundle install

EXPOSE 8000
ENTRYPOINT ["ruby"]
CMD ["app.rb", "-o", "0.0.0.0"]
