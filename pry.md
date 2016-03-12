# pry

Nesting in the prompt too noisy?

	simple-prompt

Want to display nesting level (output)

	nesting


## Debugging remotely? (e.g. Rails dev server started using foreman)

Add the following to the Gemfile under development and test

```
gem 'pry'
gem 'pry-remote'
gem 'pry-stack_explorer'
gem 'pry-debugger'
```

Then add `binding.remote_pry` where you want to pause:

```
class UsersController < ApplicationController
  def index
    binding.remote_pry
    ...
  end
end
```

### GOTCHAS

For Rails 5 beta, Here's the Gemset that works

```
group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'pry'
  gem 'byebug'
  gem 'pry-byebug', '1.3.3'
  gem 'pry-remote'
  gem 'pry-rails'
  gem 'pry-stack_explorer'
end
```
