# log-colors
### Print logs with color

This command makes sure that the logs being tailed have colored output.

Usage: 
 * save it as an alias (~/.bash_aliases)
 ** logColor="ack-grep ....."
 * then, ~$ tail -F log.log | logColor

ack-grep --flush --passthru --color --color-match=red '^.*ERROR.*' | ack-grep --flush --passthru --color --color-match=red '^.*SEVERE.*' | ack-grep --flush --passthru --color --color-match=green '^.*DEBUG.*' | ack-grep --flush --passthru --color --color-match=blue '^.*INFO.*' | ack-grep --flush --passthru --color --color-match=on_bright_white '^.*LKC.*' | ack-grep --flush --passthru --color --color-match=magenta '^.*ception.*' | ack-grep --flush --passthru --color --color-match=magenta '^.*	at.*'

