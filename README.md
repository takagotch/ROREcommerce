### ROREcommerce
---
http://www.ror-e.com/

https://github.com/drhenner/ror_ecommerce

```
gem install bundler
bundle install
rake secret # copypaste the output as `encryption_key` in `config/settings.yml`
rake db:create:all
rake db:migrate db:seed
RAILS_ENV=test rake db:test:prepare
RAILS_ENV=test rake db:seed


FOG_DIRECTORY => your bucket on AWS
AWS_ACCESS_KEY_ID => your access key on AWS
AWS_SECRET_ACCESS_KEY => your secret key on AWS
AUTHNET_LOGIN => if you use authorize.net otherwise change config/settings.yml && config/environments/*.rb
AUTHNET_PASSWORD => if you use authorize.net otherwise change config/settings.yml && config/environments/*.rb

export FOG_DIRECOTRY=xxxxxx
export AWS_ACCESS_KEY_ID=xxxxxxx
export AWS_SECRET_ACCESS_KEY=xxxxxxxx
export AUTHNET_LOGIN=xxxxxxx
export AUTHNET_PASSWORD=xxxxxxxxx

heroku config:add FOG_DIRECTORY=xxxxxx
heroku config:add AWS_ACCESS_KEY_ID=xxxxxx
heroku config:add AWS_SECRET_ACCESS_KEY=xxxxxx
heroku config:add AUTHNET_LOGIN=xxxxxx
heroku conifg:add AUTHNET_PASSWORD=xxxxxxx
heroku labs:enable user-env-compile -a myapp
heroku config:add SENGRID_USERNAME=xxxxx
heroku config:add SENDGRID_PASSWORD=xxxxx

rake db:seed_fake

yardoc --no-private --protected app/models/*.rb

Paperclip.options[:command_path]
# conifg/paperclip.rb
Paperclip.options[:command_path] = "/usr/local/bin"
Paperclip.options[:command_path] = "/usr/local/bin"
Paperclip.options[:command_path] = "/usr/bin"

#config/initializers/session_store.rb
require 'action_dispatch/middleware/session/dalli_store'
Hadean::Application.config.session_store :dalli_store, :key => '_hadean_session_ugrdraaaaaaaa'

config.cache_store = :dalli_store

gem 'suspot_solr'
gem 'sunspot_rails'
bundleinstall
rake sunspor:solr:start
# product.rb
# include ProductSolr
def self.standard_search


<?xml version="1.0" encoding="UTF-8"?>
<CORSConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
<CORSRule>
<AllowedOrigin>*</AllowedOrigin>
<AllowedMethod>GET</AllowedMethod>
<MaxAgeSeconds>3000</MaxAgeSeconds>
<AllowedHeader>Content-*</AllowedHeader>
<AllowedHeader>Host</AllowedHeader>
</CORSRule>
</CORSConfiguration>



```

