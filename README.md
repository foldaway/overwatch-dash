# Overwatch Dashboard
[![CircleCI](https://circleci.com/gh/bottleneckco/overwatch-dashboard/tree/master.svg?style=shield)](https://circleci.com/gh/bottleneckco/overwatch-dashboard/tree/master) [![Code Climate](https://codeclimate.com/github/bottleneckco/overwatch-dashboard/badges/gpa.svg)](https://codeclimate.com/github/bottleneckco/overwatch-dashboard) [![Test Coverage](https://codeclimate.com/github/bottleneckco/overwatch-dashboard/badges/coverage.svg)](https://codeclimate.com/github/bottleneckco/overwatch-dashboard/coverage) [![Issue Count](https://codeclimate.com/github/bottleneckco/overwatch-dashboard/badges/issue_count.svg)](https://codeclimate.com/github/bottleneckco/overwatch-dashboard)

Web app that displays competitive statistics for a selection of Overwatch players.

## Dependencies
- `$ bundle install`
- `$ yarn`

## Development
### Database setup
1. Run `$ rake db:setup`
2. Run:  
`$ foreman start -f Procfile.dev`
3. Access [http://localhost:5000](http://localhost:5000). (There'll likely be output from foreman on port 8080 but that is for `webpack-dev-server`)

## Production
If you ever need to run the assets compilation that is used for production, run:  
`$ bundle exec rake NODE_ENV=production RAILS_ENV=production assets:precompile --trace`

## Architecture
The web application is written in Ruby with the Rails framework. React is used for the front-end.
