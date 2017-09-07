# FloApp

rails new floapp 


===============================================================================
Add
gem 'rails_admin', '~> 1.2'
to Gemfile
and run
bundle install

bin/rails g rails_admin:install
===============================================================================
Add
gem 'remotipart', '~> 1.2'
to Gemfile
and run
bundle install
===============================================================================
Add 
gem 'rails_admin_rollincode', '~> 1.0'
to Gemfile
and run
bundle install

===============================================================================
Add 
gem 'devise'
to Gemfile
and run
bundle install
===============================================================================
Then, run the generator
$ rails generate devise:install

Running via Spring preloader in process 11017
      create  config/initializers/devise.rb
      create  config/locales/devise.en.yml
===============================================================================

Some setup you must do manually if you haven't yet:

  1. Ensure you have defined default url options in your environments files. Here
     is an example of default_url_options appropriate for a development environment
     in config/environments/development.rb:

       config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

     In production, :host should be set to the actual host of your application.

  2. Ensure you have defined root_url to *something* in your config/routes.rb.
     For example:

       root to: "home#index"

  3. Ensure you have flash messages in app/views/layouts/application.html.erb.
     For example:

       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p>

  4. You can copy Devise views (for customization) to your app by running:

       rails g devise:views

===============================================================================


==> bin/rails generate devise User

===============================================================================

bin/rails g scaffold Category title description

bin/rails g scaffold Widget title:string description:string notes:text category:belongs_to
===============================================================================
bin/rails db:migrate

===============================================================================
Add 
gem 'devise'
to Gemfile
and run
bundle install
===============================================================================

Add 
gem 'frontend-generators'
to Gemfile
and run
bundle install


===============================================================================

## Helpful Links

http://onebitcode.com/english-rails-admin/

https://github.com/activeadmin/activeadmin/wiki

