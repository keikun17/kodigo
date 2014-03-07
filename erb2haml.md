for each erb file, convert it to Haml and removing the erb if successful.
    for file in app/views/devise/**/*.erb; do html2haml -e $file ${file%erb}haml && rm $file; done
