
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
|[Rack Canonical Host](https://github.com/tylerhunt/rack-canonical-host)|Redirect to the primary domain for the application.
|[Rack::Timeout](https://github.com/sharpstone/rack-timeout)|Timeout app so we can get notified before Heroku kills the request that runs over 30s.


### Application Monitoring 🕵️‍♂️
|Name|Details|Pricing
|--|--|--|
|[Cloudflare](https://www.cloudflare.com)|DNS service with request monitoring, DDoS protection and other security features.|[from $0/mo](https://www.cloudflare.com/en-gb/plans/)
|[RayGun](https://raygun.com)|Production app error monitoring, crash reporting & notifications.|[from $9/mo](https://elements.heroku.com/addons/raygun)
|[Skylight](https://www.skylight.io)|App performance monitoring & insights to optomise for faster app response.|[from $20/mo](https://www.skylight.io/pricing)
|[Papertrail](https://www.papertrail.com)|Server logs archive and management.|[from $8/mo](https://elements.heroku.com/addons/papertrail)
|[Lograge](https://github.com/roidrage/lograge)|Tame Rails' request logging.
|[Lograge::Sql](https://github.com/iMacTia/lograge-sql)|Extension to Lograge gem for taming SQL queries.
|[Logstop](https://github.com/ankane/logstop)|Remove personally identifiable information (PII) out of logs.


### Security 🔒
|Name|Details|Pricing
|--|--|--|
|[Sqreen](https://www.sqreen.com)|Application level security platform.|[from $0/mo](https://www.sqreen.com)
|[Rack::Attack](https://github.com/rack/rack-attack)|Block and throttle abusive requests.
|[Devise Security](https://github.com/devise-security/devise-security)|Devise gem extension to add additional security features for modern web applications.
|[Lockbox](https://github.com/ankane/lockbox)|Database fields encryption.
|[Blind Index](https://github.com/ankane/blind_index)|Securely search encrypted database fields.
|[StrongPassword](https://github.com/bdmac/strong_password)|Password strength validation. Don't allow weak passwords.
|[ValidEmail2](https://github.com/micke/valid_email2)|Validate email address, prevent disposable emails and blacklist domains.

## Rails Features

### User Accounts & Permissions 👤
|Name|Details|Pricing
|--|--|--|
|[Devise](https://github.com/heartcombo/devise)|User authentication system.
|[OmniAuth](https://github.com/omniauth/omniauth)|External provider authentication. e.g. Connect with Google, Facebook, etc.
|[Pundit](https://github.com/varvet/pundit)|User authorization system.
|[Pretender](https://github.com/ankane/pretender)|Login as any user in the platform as an admin.


### Records 💿
|Name|Details|Pricing
|--|--|--|
|[FriendlyId](https://github.com/norman/friendly_id)|Hide database row IDs and produce SEO friendly URLs.
|[PaperTrail](https://github.com/paper-trail-gem/paper_trail)|Track changes to our records for auditing and versioning.
|[ActsAsParanoid](https://github.com/ActsAsParanoid/acts_as_paranoid)|Soft delete records.
|[AASM](https://github.com/aasm/aasm)|State machine.

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
