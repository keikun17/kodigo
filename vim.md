#vim

show all loaded vimscripts

    scriptnames

change :pwd to current file's dir

    :cd %:p:h
    
resize window
    
* `CTRL-W <` : width+1
* `CTRL-W >` : widhth-1
* `CTRL-W _` : set window to max height
* `z{nr}<CR>` : height=nr

close other tabs

    :tabo

new blank split

    Normal: CTRL-Wn

output the contents of the register

    // Any mode : Ctrl-R <register>
    // example:
    
    Ctrl-R %
    // -> outputs path to current file

show vimruntime 

    :echo $VIMRUNTIME

reload .vimrc

    :so $MYVIMRC
    
source current file

    :so %

Reload all open buffers

    :buffdo e

Reload all visible windows

    :windo e
