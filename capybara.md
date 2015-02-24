# Capybara

### Telling Capybara to run chrome instead of firefox

Install chromedriver

    brew install chromedriver

Add these lines to the boot file. On Rails, maybe `features/support/env.rb`

    Capybara.register_driver :chrome do |app|
      Capybara::Selenium::Driver.new(app, :browser => :chrome)
    end

    Capybara.javascript_driver = :chrome

### Executing JS code in the page

    // page.execute_script('some_js_code') 
    // example :
    page.execute_script('$("#hidden_thing").show()') 

### To trigger mouse events when 'capybara-webkit' gem is installed

    Rspec.configure.do |config|
      #...
      Capybara.javascript_driver =:webkit
    end

    page.find('#something').trigger(:mouseover)

### Test contents of new window opened by clicking a link / pressing a button.

    new_window = window_opened_by { click_link "Call DR House (Opens a new tab)" }

    within_window(new_window) do

      # To check that there is a pop up
      page.driver.browser.window_handles.length.should == 2

      expect(page).to have_text("It's not lupus")

    end
