# Personal System Environment Variable Changer

This is a simple Python tool used for changing values of system environment variables from the command line. This tool can be used for scripts that run under various job schedulers (such as cron).

Help prints all the available variables and their information :

- Which file uses them
- Description
- Possible values

## Use

Basic use example :

```senvch VARIABLE NEW_VALUE```

Currently the path to the file with the variables needs to be hard coded into the Python script, this is done by changing the value to the global variable :

- ```PATH_TO_FILE```

Variables should be written in the same format as the example down below. Currently the script will exit if it is not in this format.

```VARIABLE_NAME=VALUE # SCRIPT &&& DESCRIPTION &&& POSSIBLE VALUES```

### Additional Information

When changing the values of variables that represent paths make sure to surround the path with \\" and not just \". An example is down below :

- ```senvch PATH_VARIABLE \"/bin/something\"```

## Future Changes

- Multiple paths to files with variables, which are saved in a file, not just one hardcoded path
- A way to display and remove the paths
- Help should print in which file the variable is declared
- Prevent crashing/exiting when the variable information is not present/formatted incorrectly, it should only warn
- Implement some kind of optional checking if the new value is a possible value for this variable
- Implement a way, where variables can be tabbed in
- Quite option, where it doesn't print the old value
