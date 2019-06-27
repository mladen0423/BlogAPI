# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


rails new [api_name]  — api
  you can use -d [database] if you don’t wanna use sqlite3
cd [api_name]
mkdir app/controllers/api
mkdir app/controllers/api/v1

rails g scaffold Article title:string content:text slug:string
rails db:migrate

mv app/controllers/articles_controller.rb app/controllers/api/v1

update app/controllers/api/v1/articles_controller.rb file
update config/routes.rb file

rails db:seed

