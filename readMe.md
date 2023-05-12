GPG SUCCESS!

## Some hiccups that I've run into.

- gpg is deprecrated because now we have to use gpg2
- make sure to update gnupg
- on terminal, use `$ export GPG_TTY=$(tty)`
- add gpg key into git global variable
- to debug, i forgot the command but you have to have git show the last error msg
  when error is thrown.

  - Instead of:
    "fatal: failed to write commit object"

  - It will show:
    "error: gpg failed to sign the data
    fatal: failed to write commit object"

- additional step `$ git config --global commit.gpgsign true`
