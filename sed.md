#sed

Basic string substitution from source file to output file 

    # example
    echo 'a b c d e f' > file1
    sed -e 's/a/x/g' file1 > file2
    cat file2 
    # >> x b c d e f
