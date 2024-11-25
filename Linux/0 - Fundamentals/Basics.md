#### Others

| NAME | DESCRIPTION                              |
| ---- | ---------------------------------------- |
| wc   | Count<br>-l > Counts the amount of lines |

#### Getting help

| NAME    | DESCRIPTION                                          |
| ------- | ---------------------------------------------------- |
| man     | Command that shows the manual for the given command. |
| apropos | Command that finds commands by keywords.             |
#### System information

| NAME     | DESCRIPTION                                                                                                                                                                |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| whoami   | Displays current username.                                                                                                                                                 |
| id       | Returns users identity                                                                                                                                                     |
| hostname | Sets or prints the name of current host system.                                                                                                                            |
| uname    | Prints basic information about the operating system name and system hardware.<br>- r > Shows Kernel version<br>- m > Shows the machine hardware name                       |
| pwd      | Returns working directory name.                                                                                                                                            |
| ifconfig | The ifconfig utility is used to assign or to view an address to a network interface and/or configure network interface parameters.                                         |
| ip       | Ip is a utility to show or manipulate routing, network devices, interfaces and tunnels.<br>- link show -> This command will list all network interfaces and their details. |
| netstat  | Shows network status.                                                                                                                                                      |
| ss       | Another utility to investigate sockets.                                                                                                                                    |
| ps       | Shows process status.                                                                                                                                                      |
| who      | Displays who is logged in.                                                                                                                                                 |
| wnv      | Prints environment or sets and executes command.                                                                                                                           |
| lsblk    | Lists block devices.                                                                                                                                                       |
| lsusb    | Lists USB devices                                                                                                                                                          |
| lsof     | Lists opened files.                                                                                                                                                        |
| lspci    | Lists PCI devices.                                                                                                                                                         |
| echo $0  | Shows current shell                                                                                                                                                        |

#### Navigation

| NAME  | DESCRIPTION                                                                                                                   |
| ----- | ----------------------------------------------------------------------------------------------------------------------------- |
| ls    | Lists the content inside a directory.<br>-l > Additional info.<br>-a > All the files, include hidden.<br>-t > Shorted by time |
| cd    | Move to the specified directory  <br>.. > Move to father<br>'blank' > Move to default                                         |
| clear | Clean the terminal                                                                                                            |

#### Files and Directories

| NAME  | DESCRIPTION                                           |
| ----- | ----------------------------------------------------- |
| touch | Create file                                           |
| mkdir | Create directory<br>-p > Create recursive directories |
| tree  | See the structure of files and directories            |
| mv    | Rename \| move a directory/file                       |
| cp    | Copy a directory or file                              |

#### Edit files

| NAME | DESCRIPTION                   |
| ---- | ----------------------------- |
| nano | Create \| Edit files          |
| vim  | Create \| Edit files          |
| cat  | Display the content of a file |
#### Find files

| NAME   | DESCRIPTION                                                                                                                                             |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| which  | Returns the path to the file or link that should be executed.                                                                                           |
| find   | To find files and folders with the capability to filter the results.<br>-type > File type<br>-name > Name hint<br>-user > User hint<br>-size +/- > Size |
| locate | Same as find, but works with an internal database, is kinnda fast but has no filters                                                                    |
##### File Descriptors and Redirections

| NAME           | DESCRIPTION                                                                                                           |
| -------------- | --------------------------------------------------------------------------------------------------------------------- |
| STDIN – 0      | Data Stream for Input                                                                                                 |
| STDIN – 1      | Data Stream for Output                                                                                                |
| STDIN – 2      | Data Stream for Output that relates to an error occurring                                                             |
| /dev/null      | Null device that discards all data<br>2>/dev/null                                                                     |
| 'Redirections' | > (File) >Redirects to a file<br>>> (File) > Adds to the existing file / content<br>< (File) > Feeds the command used |
| \| 'Pipeline'  | Redirects de output from a command to the input from the next one                                                     |
##### Filter content

| NAME   | DESCRIPTION                                                                   |
| ------ | ----------------------------------------------------------------------------- |
| more   | The output stays at the terminal                                              |
| less   | The output do not stay in the terminal                                        |
| head   | First X amount of lines                                                       |
| tail   | Last X amount of lines                                                        |
| short  | To short the results                                                          |
| grep   | To extract some results                                                       |
| tr     | To replace one character with another                                         |
| cut    | To select info delimited by some delimiters<br>> -d"{delimiter}" -f{position} |
| column | To give a basic 'column' type formatting to the output                        |
