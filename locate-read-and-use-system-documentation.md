## Locate, Read and Use System Documentation
- `man passwd` - man page for /usr/bin/passwd
- `man 5 passwd` - man page for /etc/passwd config file
- `apropos PATTERN` - finds man pages that match PATTERN
- `mandb` updates/indexes everything in /usr/share/man -- you might need to do this if `apropos PATTERN` doesn't return anything
- `info` reads from /usr/share/info
- `info COMMAND` will default to `man COMMAND` if there is no info page for COMMAND
- when inside `info` you can use '?' to get help navigating around
- `info` is a GUI, you bring the cursor to a line and press enter to move into it
- `info --apropos=PATTERN` searches for info pages matching PATTERN.
- `info coreutils tee` will bring up the info page for `tee`, under the coreutils Node.
- if a command doesn't have man or info pages, try --help, -h, or look in /usr/share/doc
- `locate passwd` searches the whole system for files related to passwd. it searches a cached database, which can be updated via `updatedb`
- `updatedb` runs once a day (default setting) via cron
- `whatis passwd` searches man page DESCRIPTIONS (not titles)
- `whereis passwd` displays location of executable AND documentation
- `rpm -q -d PACKAGE` Queries the Documentation for PACKAGE
