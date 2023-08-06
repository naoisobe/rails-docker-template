FROM ruby:3.2.2

ENV APP /app
RUN mkdir -p $APP
COPY . $APP/

RUN gem update --system && gem install bundler

WORKDIR $APP

ENTRYPOINT ["./bin/docker-entrypoint.sh"]
EXPOSE 3000
CMD ["bin/dev"]
