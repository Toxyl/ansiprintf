# ansiprintf
A small PHP script that extends sprintf with shorthands for ANSI formatting.

The idea is to extend the `sprintf` function of PHP with ANSI capabilities for terminal output under Linux. All functionality of `sprintf` should have been retained (untested though!) whilst adding a few new constructs:

## Commands
### `%rst>`
Resets all formatting. 

### `%fN>`
Sets the foreground color to an int (`N`), ranging from 0 to 255. 

### `%*N>`
Sets the foreground color to an int (`N`) ranging from 0 to 255 and prints the following **bold**. 

### `%_N>`
Sets the foreground color to an int (`N`) ranging from 0 to 255 and prints the following __underlined__. 

### `%~N>`
Sets the foreground color to an int (`N`) ranging from 0 to 255 and prints the following *italic*. 

### `%bN>`
Sets the background color to an int (`N`), ranging from 0 to 255. 

### `%fbN,M>`
Sets the foreground color to an int (`N`) and then the background color to an int (`M`), each ranging from 0 to 255. 

### `%bfN,M>`
Sets the background color to an int (`N`) and then the foreground color to an int (`M`), each ranging from 0 to 255. 

## Installation
```
cp ansiprintf /usr/local/bin/ansiprintf
chmod +x /usr/local/bin/ansiprintf
ansiprintf
```