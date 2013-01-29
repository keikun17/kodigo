#rpm

Initialize private rpm db

    rpm --initdb --root /home/username/local --dbpath /home/username/local/lib/rpm

rpm dependency check

    rpm -ivh package.rpm

Relocate rpm paths

    rpm --root /home/username/local --dbpath /home/username/local/lib/rpm --relocate /usr=/home/username/local --nodeps -ivh package.rpm
