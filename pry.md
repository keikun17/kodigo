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
