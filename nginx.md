#nginx

###Common File locations

1. /etc/nginx/nginx.conf
2. /opt/nginx/conf/nginx.conf

### nginx.conf Virtualhost Samples

##### What you probably need:
	server {
    	listen          80;
	    server_name     www.domain.com;

	    index           index.html;
	    root            /home/domain.com;
	}

##### For redirects :
	server {
    	listen          80;
	    server_name     domain.com *.domain.com;
    	return          301 $scheme://www.domain.com$request_uri;
	}





	