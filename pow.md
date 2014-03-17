Install or upgrade

    curl get.pow.cx | sh


Setup 'http://myapp.dev'

    cd ~/.pow
    ln -s /path/to/myapp

Restart rails app

    touch tmp/restart.txt

View pow access log

    tail -f ~/Library/Logs/Pow/access.log
    
View 'myapp' logs

    tail -f ~/Library/Logs/Pow/apps/myapp.log
    
