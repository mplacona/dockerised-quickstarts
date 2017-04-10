FROM ruby:latest

RUN mkdir /usr/src/app 
ADD . /usr/src/app/ 
WORKDIR /usr/src/app/ 

# Install gems
ADD Gemfile* /usr/src/app/ 
RUN bundle install

CMD ["bundle", "exec", "ruby", "-p", "3000", "app.rb"]