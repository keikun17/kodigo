#vim

change :pwd to current file's dir

    :cd %:p:h
    
resize window
    
* `CTRL-W <` : width+1
* `CTRL-W >` : widhth-1
* `CTRL-W _` : set window to max height
* `z{nr}<CR>` : height=nr

new blank split

    Normal: CTRL-Wn

output the contents of the register

    // Any mode : Ctrl-R <register>
    // example:
    
    Ctrl-R %
    // -> outputs path to current file

show vimruntime 

    :echo $VIMRUNTIME
