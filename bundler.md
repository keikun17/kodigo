#bundler

### Gemfile
For specifying a different gem collection for jruby and ruby

	platform :jruby do
		gem 'jdbc-mysql'
	end

	platform :ruby do
		gem 'mysql
	end


Bundle only the locally installed gems (and within gemset)

    bundle install --local
