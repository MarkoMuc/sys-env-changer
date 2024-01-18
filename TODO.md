# Future changes

## TODOs

- [X] TODO: The paths should be read from a file. Make it so multiple config/env variable files can be saved.
          - They get saved in $HOME/.config/senvch/paths.cfg.
	  - Each path is conjoined with a possible alias "path:alias".
          - Add a way to display all of them, the user should be able to remove them too.
- [X] TODO: Commands.
  - [X] TODO: Add paths.
	- A path or an alais can be added with "add PATH[:ALIAS] ..."
  - [X] TODO: List saved paths and aliases
	- List all paths and alaises "paths -a" or "paths --all".
	- List all path with matching alias "paths ALIAS ...".
	- Print out only aliases "paths -a -o".
  - [X] TODO: Delete paths by path or alias.
	- A path can be deleted with "delete PATH ...".
	- An alais can be deleted with "delete -a ALIAS ...".
  - [X] TODO: Delete all occurances of an alias.
  	- An alias can be deleted with "delalias ALIAS ...".
  - [X] TODO: Change all occurances of an alias.
	- An alais can be changed with "change ALIAS ALIAS".
  - [X] TODO: List variables.
	- List variables in selected config files by path or ALIAS "vars (PATH|ALIAS)...".
	- List all variables in all config files "vars -a".
  - [X] TODO: Changing values.
	- Change the value of a variable "edit (PATH|ALIAS) VARIABLE VALUE".
  - [X] TODO: Working with file paths that are not saved.
	- Print all variables in a file "file -a PATH".
	- Change variable in a file "file PATH -c VARIABLE VALUE".
- [X] TODO: Prevent it from crashing when description is not present/not formatted correctly.
      - make it so it just gives a warning for those files.
- [X] TODO: Quite option, where it doesn't print the old value -> or just make current option as the verbose one.
- [ ] TODO: Testing

## Quick Fix

- [X] Add stderr stream
- [X] Fix deleting
- [X] If multiple = in variable name and value combo, just combine them as the value
- [X] Same for splitting with #
- [X] Same var name means overwritting
- [X] Add argument -n to add, when you dont want to change an existing path:alias combo 

## Ideas

Maybe add also the ability to change the description and name of the variable.

Since editing values is supposed to be the main thing, maybe edit should be the default command and others are the subcommands.

Future release:
- Add regex searching.

