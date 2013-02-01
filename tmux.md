#tmux

Swap window order

    <prefix> :swap-window -s <tab1#> -t <tab2#>

Clear screen

    <prefix> :send-keys -R
    
Clear scrollback

    <prefix> :clear-history

Log out other sessions in the current window (maybe bad sessions that causes window size to get stuck)

    <prefix> D
