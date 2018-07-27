Commands

|                      | Ruby/Rake/Rails                            | Elixir/Mix/Phoenix                        |
|----------------------|--------------------------------------------|------------------------------------------|
| start server         | rails s -b 0.0.0.0                         | mix.server                               |
| create migration     | rails g migration create_games_users_table | mix ecto.gen.migration create_games_user |
| run migration        | bundle exec rake db:migrate                | mix ecto.migrate                         |
| rollback migration   | rails db:rollback                          | mix ecto.rollback                        |
| rails console        | rails c                                    | iex -S mix                               |
|                      | rake routes                                | mix phoenix.routes                       |
| install dependencies | bundle install # from Gemfile              | mix deps.get # from  mix.exs             |
| current rails version| rails --version                            | mix phoenix.new --version                |

Interactive Shell

|                      | irb                                        | iex                                      |
|----------------------|--------------------------------------------|------------------------------------------|
| break trigger        | <Ctrl-C>                                   | iex(1) > #iex:break                      |

Models

|                      | Rails/ActiveRecord                         | Repo                                     |
|----------------------|--------------------------------------------|------------------------------------------|
| Find All             | User.all                                   | Repo.all(User)                           |
| Find by ID           | User.find(1)                               | Repo.get!(User, 1)                       |
| Find by field        | User.where(username: "kapitolin")          | Repo.get_by(User, username: "kapitolin") |


Generate Scaffold
---

Rails :

```
rails g scaffold ModelName field:type
# $ rails generate scaffold HighScore game:string score:integer
```

Elixir :

```
mix phoenix.gen.html ModelName modelname_pluraized field:type
# $ mix phoenix.gen.html Video videos user_id:references:user url:string title:string description:text
```



