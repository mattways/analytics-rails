[![Gem Version](https://badge.fury.io/rb/analytics-rails.svg)](http://badge.fury.io/rb/analytics-rails)
[![Code Climate](https://codeclimate.com/github/mmontossi/analytics-rails/badges/gpa.svg)](https://codeclimate.com/github/mmontossi/analytics-rails)
[![Build Status](https://travis-ci.org/mmontossi/analytics-rails.svg)](https://travis-ci.org/mmontossi/analytics-rails)
[![Dependency Status](https://gemnasium.com/mmontossi/analytics-rails.svg)](https://gemnasium.com/mmontossi/analytics-rails)

# Analytics Rails

Adds a helper to create the google analytics script in rails.

## Why

I did this gem to:

- Have a simple but versatile way to include google analytics.

## Install

Put this line in your Gemfile:
```ruby
gem 'analytics-rails'
```

Then bundle:
```
$ bundle
```

## Usage

In your layout add a line like this in your head or before close body:
```erb
<%= google_analytics_include_tag 'your-id', variable: 'value' %>
```

And custom events after the include tag:
```erb
<%= google_analytics_event_tag 'popup', 'click' %>
```

NOTE: Will only show the tags in production environment.

## Credits

This gem is maintained and funded by [mmontossi](https://github.com/mmontossi).

## License

It is free software, and may be redistributed under the terms specified in the MIT-LICENSE file.
