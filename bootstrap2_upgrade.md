# Bootstrap 2 to Bootstrap 3 cheatsheet

"slash" search '/' for Bootstrap 2.x spans (e.g. span1..span12) within the file.

    /span\d

replace all Bootstrap 2.x `spanxx` to bootstrap 3.x `col-sm-xx` within the file

    :%s/span\(\d\)/col-sm-\1/gc
