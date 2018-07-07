|                      | Ruby/Rake/Rails                            | Elixir/MixPhoenix                        |
|----------------------|--------------------------------------------|------------------------------------------|
| start server         | rails s -b 0.0.0.0                         | mix.server                               |
| create migration     | rails g migration create_games_users_table | mix ecto.gen.migration create_games_user |
| run migration        | bundle exec rake db:migrate                | mix ecto.migrate                         |
| rails console        | rails c                                    | iex -S mix                               |
|                      | rake routes                                | mix phoenix.routes                       |
| install dependencies | bundle install # from Gemfile              | mix deps.get # from  mix.exs             |
