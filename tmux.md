#tmux

Swap window order

    <prefix> :swap-window -s <tab1#> -t <tab2#>

Clear screen

    <prefix> :send-keys -R

Clear scrollback

    <prefix> :clear-history

Log out other sessions in the current window (maybe bad sessions that causes window size to get stuck)

    <prefix> D

Maximize Pane (to minimize pain in small screens)

    <previx> z

Reload source

    :source-file ~/.tmux.conf

Sessions
----

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
