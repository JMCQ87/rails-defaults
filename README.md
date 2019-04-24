# Default "Template" Rails App

Do you have yet ANOTHER coding challenge to do? Hackathon? New project to start? I know I do! ;)

Hence, to make some things easier, I decided to create this "rails new"-with-some-defaults app "template" of sorts, with the most notable defaults being Postgres (instead of SQLite) as the database and RSpec (instead of Minitest) for testing.

Partially, this idea has been inspired by Claudia Romano's [Medium Post on a related topic](https://medium.com/@cromano31415/how-to-build-a-new-rails-app-with-rspec-postgresql-and-git-1d33c7e60456).

## What I decided to include & Why

### DB & Testing
* Postgres: As I prefer to use the same type of database locally as in production and I do not like SQLite much.
* RSpec: Because I have not really used Minitest since 2015 and it's much more widely adopted.

### Other Gems
* Faraday: To have a well-maintained HTTP library included that I am familiar with, because so far almost all my projects have ended up making external calls at some point. (httparty would have been my top alternative. Split-decision, might make a switch here in the future.)
* Rubocup: Because I want to pay attention to a good Ruby coding style in all my future projects.

## What I left OUT & Why

### Code
* Any sort of actual (template) implementation: I also do not intend to add that in the future, as I see very limited value in that.

### Gems
* httparty: See Faraday above.
* Devise: Users have been a frequent occurrence in my projects as well
* ActiveAdmin: Done most of my Ruby work around this in the last couple years, but I am doubtful I am going to use it again for a new project.
