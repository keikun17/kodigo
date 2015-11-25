# find
Recursively Find all subdirectories of a particular name from the current within the current path

	find . -name 'dirname_in_regex*' -type -d


Recusively grep through files within the directory to find a matching string

	find . -type f -exec grep -il "hello" {} \;


Recusively grep through files with a given extension within the present directory to find matching strings

	find . -type f -name "*.ext" -exec grep -il "hello" {} \ 

find all new files created within 24 hours
	
	find . -newerBt "24 hours ago" 
	
set and persist environment variable

    set -U SECREY_KEY sUp3rsecretK3y
