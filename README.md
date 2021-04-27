

# 🛤🚂 Rails Stack
Our preferred list of commonly used Ruby gems, tools &amp; services we like to use for our Rails platforms. 


# 💎 Gems, Libraries & Services

Pricing below are for a small to medium sized production application with more than 100 active users. Most external service's pricing are based on usage so will vary based on popularity of the app. 

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
|[SendGrid](http://sendgrid.com)|Transactional email delivery.|[from $15/mo](https://sendgrid.com/pricing/)


### Application Monitoring 🕵️‍♂️
|Name|Details|Pricing
|--|--|--|
|[Cloudflare](https://www.cloudflare.com)|DNS service with request monitoring, DDoS protection and other security features.|[from $0/mo](https://www.cloudflare.com/en-gb/plans/)
|[HoneyBadger](https://www.honeybadger.io)|Production app monitoring, crash reporting & notifications.|[from $0/mo](https://www.honeybadger.io/plans/)
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
|[Paranoia](https://github.com/rubysherpas/paranoia)|Soft delete records.
|[AASM](https://github.com/aasm/aasm)|State machine.

### Front-end Helpers 🚇
|Name|Details|Pricing
|--|--|--|
|[HAML](https://github.com/haml/haml-rails)|HTML abstraction markup language to keep the code simple and indented like Ruby.
|SASS|Rails built-in support for CSS with superpowers.
|[Pagy](https://github.com/ddnexus/pagy)|Pagination.
|[Simple Form](https://github.com/heartcombo/simple_form)|Form components & styling.
|[High Voltage](https://github.com/thoughtbot/high_voltage)|Static pages.
|[MetaTags](https://github.com/kpumuk/meta-tags)|Page titles, descriptions and meta tags for SEO. 
|[SitemapGenerator](https://github.com/kjvarga/sitemap_generator)|Generate sitemaps for search engines.
|[Gon](https://github.com/gazay/gon)|Pass data as variables from backend to Javascript.
|[Hotwire: Turbo](https://turbo.hotwire.dev)|Speed of single-page web application.
|[Hotwire: Stimulus](https://stimulus.hotwire.dev)|Modest JavaScript framework for HTML.


## Internal

### Platform Administration 👨‍💼
|Name|Details|Pricing
|--|--|--|
|Option 1: [Forst Admin](https://www.forestadmin.com)|Admin panel as a service.|[from $0/mo](https://www.forestadmin.com/pricing/)
|Option 2: [Active Admin](https://github.com/activeadmin/activeadmin) & [Addons](https://github.com/platanus/activeadmin_addons)|Admin panel as part of the Rails app.


### Code Quality 👾
|Name|Details|Pricing
|--|--|--|
|[Rubocop](https://github.com/rubocop/rubocop)|Ruby static code analyzer and code formatter. Install auto-correct plugin in your code editor.
|[Deep Source](https://deepsource.io)|Automated code review & static code analysis. Setup Rubycop, [Breakman](https://github.com/presidentbeef/brakeman) and other code review plugins for each PR.|[from $0/mo](https://deepsource.io/pricing/)
|[Strong Migrations](https://github.com/ankane/strong_migrations)|Catch unsafe migrations in development.
|[Bullet](https://github.com/flyerhzm/bullet)|Improve app performance by reducing the number of queries it makes.

### Automated Testing 🧪
|Name|Details|Pricing
|--|--|--|
|[RSpec](https://github.com/rspec/rspec)|Testing framework.
|[factory_bot](https://github.com/thoughtbot/factory_bot)|Define model patters and strategies for testing. 
|[Faker](https://github.com/faker-ruby/faker)|Mock test data.
|[Shoulda Matchers](https://github.com/thoughtbot/shoulda-matchers)|One-liner common Rails functionality tests helper.
|[Capybara](https://github.com/teamcapybara/capybara)|User acceptance testing by simulating how real users would interact with our app.
|[GitHub Actions](https://github.com/features/actions)|Continuous Integration (CI) setup for each PR.|[3,000 mins/mo](https://github.com/pricing) included with GitHub subscription.


### Development Tools 🛠
|Name|Details|Pricing
|--|--|--|
|[GitHub Teams](https://github.com/team)|Codebase, version control & developer hub.|[$4 per user/mo](https://github.com/pricing)
|[Better Errors](https://github.com/pricing)|Better and more useful error pages.
|[Awesome Print](https://github.com/awesome-print/awesome_print)|Pretty print logs and indentation.
|[Annotate](https://github.com/ctran/annotate_models)|Add summarizing schema as comments for quick reference at the top of files.
|[Letter Opener](https://github.com/ryanb/letter_opener)|Open and view emails in the browser in development.
