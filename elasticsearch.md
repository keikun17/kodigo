elasticsearch
----

File locations when installed with brew

    You'll find the ElasticSearch log here:
        open /usr/local/var/log/elasticsearch/elasticsearch_Mengsk.log

    The folder with cluster data is here:
        open /usr/local/var/elasticsearch/elasticsearch_Mengsk/

    You should see ElasticSearch running:
        open http://localhost:9200/

    ==> Caveats
    To have launchd start elasticsearch at login:
        ln -sfv /usr/local/opt/elasticsearch/*.plist ~/Library/LaunchAgents
    Then to load elasticsearch now:
        launchctl load ~/Library/LaunchAgents/homebrew.mxcl.elasticsearch.plist
    Or, if you don't want/need launchctl, you can just run:
        elasticsearch -f -D es.config=/usr/local/opt/elasticsearch/config/elasticsearch.yml
