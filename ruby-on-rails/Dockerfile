FROM ruby
LABEL maintainer="Benedict Hazel <bwhazel@gmail.com>"

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y sqlite3
RUN gem install rails bundler
EXPOSE 3000