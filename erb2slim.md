for each erb file, convert it to Slim and remove the erb if successful.

    for file in app/views/devise/**/*.erb; do erb2slim $file ${file%erb}slim && rm $file; done
