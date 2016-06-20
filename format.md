# Format

## Tangle files
The idea comes from org-mode of emacs where you can create files using
literate programming. The scripts use markdown as the base
format. Scripts can be embedded within code quotes.

``` sh file:$HOME/.bashrc
PATH=$PATH:${HOME}/bin
PS1="\w \$"
```

The above example shows how I track .bashrc file using the text
files. Executing `tangle format.md` it would create a file named
`.bashrc` under your `$HOME` directory. 

A few options are currently available:

`mkdirp:[yes|no]`: recursively creates directory if not present,
defaults to no
`tangle:[yes|no]`: whether to write the file, defaults to yes
`append:[yes|no]`: whether to append to the file or not, defaults to yes
`file`: provide file name to tangle to
