# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things I may want to cover:

* Ruby version: ruby 2.5.1p57 (2018-03-29 revision 63029) [x86_64-linux-gnu]

* System dependencies: devise, activeadmin

* Configuration:

	before deployment set @site_title in the aaplication.html.erb file
	 in development.rb set myapp to the appname -> config.action_mailer.default_url_options = { host: 'myappp.herokuapp.com', port: 3000 }

	 for using gmail as your mail gateway:
	create an app password by enabling 2-step authentication
	 and usign this page: https://myaccount.google.com/apppasswords

	for deployment on Heroku set Heroku config variables for google services:
		heroku config:set GOOGLE_CREDENTIALS="$(<../keys/adhoc-gcs-key.json)" -a app_name
		heroku config:set GMAIL_DOMAIN="your.domain.com" -a app_name
		heroku config:set GMAIL_USERNAME="username@your.domain.com" -a app_name
		heroku config:set GOOGLE_SECRET="YourAppPassword" -a app_name

* Database creation: postgres in production for Heroku and sqlite3 for testing and development

* Database initialization: db:seed that sucker and get started

* How to run the test suite: ToDo

* Services (job queues, cache servers, search engines, etc.): Umm Yeah..

* ...
May need these later...
		heroku config:set GOOGLE_PRIVATE_KEY_ID="Private key ID from keyfile" -a app_name
		heroku config:set GOOGLE_PRIVATE_KEY="Private key from keyfile" -a app_name
		heroku config:set GOOGLE_CLIENT_EMAIL="email of the service account" -a app_name
