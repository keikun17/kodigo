#vim

show all loaded vimscripts

    scriptnames

change :pwd to current file's dir

    :cd %:p:h

Find out what keystroke combination does and where it was set

    :verbose map {keystroke}      // :verbose map <C-b>

resize pane

* `CTRL-W <` : width+1
* `CTRL-W >` : widhth-1
* `CTRL-W _` : set window to max height
* `z{nr}<CR>` : height=nr
* `CTRL-_` : set pane heights to max
* `CTRL-=` : set pane heights in the same column to be equal

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

vimcrypt / encyrpt things

    :X

Profiling vim's startup and first opening of a file

    // vim --startuptime logfile.log firstfile.rb
    // then `:tabe logfile.log` to open log
    vim --startuptime startup.log config/application.rb

Finding out which .vim file has set a map

    :verbose map [keycombo]
    
## Fold

Unfold everything

    zR
