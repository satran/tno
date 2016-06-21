# Format

## Tangle files
The idea comes from org-mode of emacs where you can create files using
literate programming. The scripts use markdown as the base
format. Scripts can be embedded within comments:

<!--- shell file:/tmp/a/hello append:no mkdirp:yes-->
```
PATH=$PATH:${HOME}/bin
PS1="\w \$"
```

The above example shows how I track a temporary file using text
files. Executing `tangle format.md` it would create a file named
`hello` under your `/tmp/a` directory. 

A few options are currently available:

`mkdirp:[yes|no]`: recursively creates directory if not present,
defaults to no

`tangle:[yes|no]`: whether to write the file, defaults to yes

`append:[yes|no]`: whether to append to the file or not, defaults to yes
`file`: provide file name to tangle to

Parameters can be added globally by adding global comments such as:
<!---@ 
file:/tmp/hello
append:yes
mkdirp:yes
-->
```
hello world
```

It would be wise to keep the global settings the beginning of the file
as they are set when tangle reads them.
