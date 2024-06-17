ARG RUBY_VERSION=3.3.3

FROM ruby:${RUBY_VERSION}-slim
WORKDIR /code

RUN apt-get update
RUN apt-get install build-essential bash -y

ENV BUNDLE_PATH=/gems
COPY Gemfile /code/Gemfile
COPY Gemfile.lock /code/Gemfile.lock
RUN bundle install --jobs 4 --retry 5
COPY . /code

RUN gem install pry solargraph

CMD [ "bash" ]
