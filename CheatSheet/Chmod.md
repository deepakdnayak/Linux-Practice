# Chmod Shell Commands
chmod [options] [mode] [File_name] 

## Options
| options       | Description                          |
| ------------- | ------------------------------------ |
| -R | permission change recursively |
| -v | display a message for each file that is processed |
| -c | only displays messages for files whose permission is changed |
| -f | It helps in avoiding display of error messages. |
| -h | Change the permissions of symbolic links instead of the files they point to. |

## Mode
| Operators     | Description                          |
| ------------- | ------------------------------------ |
| + | Add permissions |
| - | Remove permissions |
| = | Set the permissions to the specified values |

## Mode
| Letters       | Description                          |
| ------------- | ------------------------------------ |
| r | Read permission |
| w | Write permission |
| x | Execute permission |

## Mode
| References    | Description                          |
| ------------- | ------------------------------------ |
| u | Owner |
| g | Group |
| o | Others |
| a | All |

## Examples
| Command       | Uses                                 |
| ------------- | ------------------------------------ |
| chmod u+rwx [file_name] | Read, write and execute permissions to the file owner |
| chmod go-w [file_name] | Remove write permission for the group and others |
| chmod u+rw,go+r [file_name] | Read and write for Owner, and Read-only for the group and other |

## Octal Permission Specification
| Binary | Octal | Permission |
| ------------- | ---------------- | ------------------- |
| 000 | 0 | - - - |
| 001 | 1 | - - x |
| 010 | 2 | - w - |
| 011 | 3 | - w x |
| 100 | 4 | r - - |
| 101 | 5 | r - x |
| 110 | 6 | r w - |
| 111 | 7 | r w x |

## Examples
| Command       | Uses                                 |
| ------------- | ------------------------------------ |
| chmod 674 [file_name] | give read and write permission to the file Owner. Read, write and executable permission to the Group. Read-only permission to the Other |