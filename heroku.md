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
