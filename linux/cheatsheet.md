# Linux Commands Cheat Sheet

Welcome to the Linux Commands repository. Essentials, Interesting and frequently-used commands describes here.

## File & Directory Operations

    pwd - Print working directory. Displays the absolute path of your current location.
    ls -la - List all files. Shows hidden files.

## Permissions & Network

    chmod Owner|Group|Other <file> - Change file permissions

### Little explain
 
    chmod 755 stand for Read, Write and Execute for Owner; Read and Execute for Group and Other.
    We can change it with simply math.: 1 is Execute, 2 is Write and 4 is Read.

A collection of essential, useful, and frequently used Linux commands with explanations and practical examples.

## File & Directory Operations

### ls 
    
    LS lists the contents of your current working directory. 
    
    ls [OPTIONS] [FILE | FOLDER]
    
    List all files in a  Linux directory including hedden (dot) files and directories.
    [xxx@xxx $] ls -a

    Human readable -Size in MB or GB
    [xxx@xxx $] ls -h 

    List files and shows permissions, user owner, group owner, and more.
    [xxx@xxx $] ls -l 

    
