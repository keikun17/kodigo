heroku
----


login with heroku credentials

    heroku login
    
initialize app for heroku

    cd my_app
    heroku create
    
deploy

    git push heroku master
    
open heroku url for current dir's heroku app

    heroku open
    
stream heroku app's production log

    heroku logs --tail

Run `rake db:seed` on Heroku

    heroku run rake db:seed
    
Set an environment var on heroku

    heroku config:set SECRET_KEY_BASE='secretkeybasehere'

Run remote command

    heroku run rake db:migrate
    heroku run rake db:version
    heroku run rake update_profiles
    
