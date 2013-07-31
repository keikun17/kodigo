#Postgres

### Here's startup instructions displayed after installing postgres with homebrew

To have launchd start postgresql at login:

    ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents

Then to load postgresql now:

    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist

Or, if you don't want/need launchctl, you can just run:

    pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start
