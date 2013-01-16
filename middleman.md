# middleman

Install

	gem install middleman
	
initialize project

	middleman init project_name
	middleman init project_name --template=html5

show all available middleman tempaltes

    middleman init --help

start server

	bundle exec middleman
	bundle exec middleman server -p 3001
	
export static version

	bundle exec middleman build