# Default "Template" Rails App

Do you have yet ANOTHER coding challenge to do? Hackathon? New project to start? I know I do! ;)

Hence, to make some things easier, I decided to create this "rails new"-with-some-defaults app "template" of sorts, with the most notable defaults being Postgres (instead of SQLite) as the database and RSpec (instead of Minitest) for testing.

Partially, this idea has been inspired by Claudia Romano's [Medium Post on a related topic](https://medium.com/@cromano31415/how-to-build-a-new-rails-app-with-rspec-postgresql-and-git-1d33c7e60456). Essentially, this is a 'rails new rails-defaults -T -d postgresql', with some additions down the line.


## Steps to do after cloning this Repo
* /config/database.yml: Change the database names and production username and password config there from rails-defaults* to the appropriate project name. Optionally, also chnage it for the other environments.
* .ruby-gemset: If you use RVM, set the correct gemset name here.
* /app/views/layouts/application.html.erb: Set the Browser title for you app.
* /config/application.rb: Re-name the module according to your app name.
* /config/cable.yml: set the redis channel according to your app name.
* /config/environments/production.rb: change queue_name_prefix for Active Job.
* package.json: set name according to your app name.

## What I decided to include & Why

### DB, Debug & Testing
* Postgres: As I prefer to use the same type of database locally as in production and I do not like SQLite much.
* RSpec: Because I have not really used Minitest since 2015 and it's much more widely adopted.
* Pry: As it is the better console than IRB.

### Other Gems
* Faraday: To have a well-maintained HTTP library included that I am familiar with, because so far almost all my projects have ended up making external calls at some point. (httparty would have been my top alternative. Split-decision, might make a switch here in the future.)
* Rubocup: Because I want to pay attention to a good Ruby coding style in all my future projects.

## What I left OUT & Why

### Configuration
* .ruby-gemset: The gemset name is intentionally not set, to avoid problems with using this "template" multiple times.

### Code
* Any sort of actual (template) implementation: I also do not intend to add that in the future, as I see very limited value in that.

### Gems
* httparty: See Faraday above.
* Devise: Users have been a frequent occurrence in my projects as well
* ActiveAdmin: Done most of my Ruby work around this in the last couple years, but I am doubtful I am going to use it again for a new project.
