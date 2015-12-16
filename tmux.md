#tmux

Swap window order

    <prefix> :swap-window -s <tab1#> -t <tab2#>

Clear screen

    <prefix> :send-keys -R

Clear scrollback

    <prefix> :clear-history

Log out other sessions in the current window (maybe bad sessions that causes window size to get stuck)

    <prefix> D

Reload source

    :source-file ~/.tmux.conf
    
Panes
-----
Maximize Pane (to minimize pain in small screens)

    <previx> z

Switch Pane positions

    <prefix> {
    <prefix> }
    
Move Pane to its own window

    <prefix> !
    
Show Pane number

    <prefix> q
Move Pane to another existing window

    // <tmux command mode>
    :move-pane -t :TARGET_WINDOW_NUM.NEW_PANE_NUMBER  // use <prefix-q> to find pane number
    // Example : To move current pane to window 1
    // :move-pane -t :1.1



Sessions
----

Create named sesion

    $ tmux new -s <session-name>
    
Rename current session

    <prefix> $ 

list sessions

    tmux ls
    # or
    tmux list-sessions

Attach to a numbered session

    tmux attach-session -t <session_number>

Start a named session

    tmux new -s <session_name>

Attach to a named session

    tmux attach -t <session_name>

Switch to a named session

    tmux switch -t <session_name>
    

Detaching Sessions
----

Detach all other sessions except current

    tmux detach -a

Select a session to detach

    <prefix>D
