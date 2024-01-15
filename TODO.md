# Future changes

## TODOs

- [X] TODO: The paths should be read from a file. Make it so multiple config/env variable files can be saved.
          - They get saved in $HOME/.config/senvch/paths.cfg 
	  - Each path is conjoined with a possible alias "path:alias"
          - Add a way to display all of them, the user should be able to remove them too
- [ ] TODO: Commands
  - [X] TODO: Add paths
	- A path or an alais can be added with "add -p PATH[:ALIAS] ..."
  - [X] TODO: List saved paths and aliases
	- List all paths and alaises "paths -a" or "paths --all"
	- List all path with matching alias "paths ALIAS ..."
	- Print out only aliases "paths -a -o"
  - [X] TODO: Delete paths by path or alias
	- A path can be deleted with "delete PATH ..."
	- An alais can be deleted with "delete -a ALIAS ..."
  - [X] TODO: Delete all occurances of an alias
  	- An alias can be deleted with "delalias ALIAS ..."
  - [X] TODO: Change all occurances of an alias
	- An alais can be changed with "change ALIAS ALIAS"
  - [X] TODO: List variables
	- List variables in selected config files by path or ALIAS "vars (PATH|ALIAS)..."
	- List all variables in all config files "vars -a"
  - [ ] TODO: Working with file paths that are not saved
	- Print all variables in a file "file -a PATH"
	- Change variable in a file "file PATH -c VARIABLE VALUE"
  - [ ] TODO: Changing values
	- Change the value of a variable "edit PATH VARIABLE VALUE"
	- Change the value of a variable by alias "edit ALIAS VARIABLE VALUE"
- [ ] TODO: Prevent it from crashing when description is not present/not formatted correctly
      - make it so it just gives a warning for those files
- [ ] TODO: Implement at least some kind of checking, if the new value is actually a possible value for this variable
      - This can be made optional
- [ ] TODO: Quite option, where it doesn't print the old value -> or just make current option as the verbose one
- [ ] TODO: Testing
	- [X] Add stderr stream
	- [ ] Fix deleting
## Ideas

Should you be able to have multiple of the same alias? -> yes!
One alias can be used on mulitple paths, so they can be bunched up by functionality.

When filling the dictionary, if an alias is used, parse the config file for all paths connected to it.

Maybe add also the ability to change the description and name of the variable.
