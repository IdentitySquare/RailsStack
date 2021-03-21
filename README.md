
# 🛤🚂 Rails Stack
Our preferred list of commonly used Ruby gems, tools &amp; services we like to use for our Rails platforms. 


# 💎 Gems, Libraries & Services

All pricing below are for a small to medium sized production application with more than 100 active users. 

## Server

### Data Storage ☁️
|Name|Details|Pricing|
|--|--|--|
|[PostgreSQL](https://www.digitalocean.com/community/tutorials/how-to-set-up-ruby-on-rails-with-postgres)| Our primary SQL database for record storage. |
|[Redis](https://opensource.com/article/18/4/ruby-rails-redis)|  Used for cache, jobs queue.
|~~Active Storage~~| Rails supported file record storage. 
|[Filestack](https://github.com/filestack/filestack-rails)| We prefer Filestack to handle all security and manage the file upload experience where uploading files is a cruitial part of the application.|[from $49/mo](https://www.filestack.com/pricing/)

### Hosting 🌎
|Name|Details|Pricing
|--|--|--|
|[Heroku](https://www.heroku.com/home)|Fully managed Platform as a Service (PaaS) by Salesforce. HIPAA, ISO & SOC [complient](https://www.heroku.com/compliance) hosting services. 1x standard web dyno, 1x standard worker dyno.| [from $50/mo](https://www.heroku.com/pricing)
|[Heroku Postgres](https://www.heroku.com/postgres)|Fully managed database as a service.|[from $9/mo](https://elements.heroku.com/addons/heroku-postgresql)
|[Heroku Redis](https://elements.heroku.com/addons/heroku-redis)|Redis as a service.|[from $0/mo](https://elements.heroku.com/addons/heroku-redis)
|[Heroku Scheduler](https://elements.heroku.com/addons/scheduler)|Tasks that need to run at regular intravels or at a particualr time everyday.|free
|[Sidekiq](https://github.com/mperham/sidekiq)|Simple & efficient background processing.
|[Rack Canonical Host](https://github.com/tylerhunt/rack-canonical-host)|

* Heroku
* Heroku Postgres
* Heroku Scheduler
* Redis Server
* Sidekiq
* rack-cononical-host
* rack-timeout

### Application Monitoring 🕵️‍♂️
* Cloudflare
* raygun
* Sqreen
* Skylight
* Papertrail
* lograge, lograge-sql
* logstop


### Security 🔒
* devise security
* blind_index
* lockbox
* strong_password
* rack-attack


## Rails Features

### User Accounts & Permissions 👤
|Name|Details|Pricing
|--|--|--|

* Devise
* Omniauth (Google + Facebook)
* Pundit
* strong password
* pretender
* valid_email2

### Records 💿
* Friendly IDs
* paper_trail
* acts_as_paranoid
* AASM

### Front-end Helpers 🚇
* Kaminari
* bootstrap4_kaminari-views
* sitemap_generator
* HAML
* SASS
* Simple Forms
* High Voltage
* Meta-tags
* Gon


## Internal

### Platform Administration 👨‍💼
* Active Admin
* Activeadmin_addons
* Maily

### Code Quality 👾
* Strong migrations
* Breakman
* Rubocop
* Codeclimate

### Automated Testing 🧪
* RSPEC
* Shoulda matchers
* Factory Bot
* Faker
* Capybara 
* Github actions for CI

### Development Tools 🛠
* Better errors
* awesome print
* Hirb
* Bullet
* Peek
* Annotate
* Letter opener 
* Phrase
