# Capybara

### Telling Capybara to run chrome instead of firefox

Install chromedriver
>`brew install chromedriver`

Add these lines to the boot file. On Rails, maybe `features/support/env.rb`
>`Capybara.register_driver :chrome do |app|`
>>`Capybara::Selenium::Driver.new(app, :browser => :chrome)`
>`end`

>`Capybara.javascript_driver = :chrome`


