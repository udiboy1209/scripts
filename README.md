Scripts
======

Collection of scripts I need for various purposes

### `rclink` and `rcunlink`

They work like GNU/stow but are extremely simple and only use soft-links.
They are used to manage sets of softlinked files, like configs etc.
You can store 'linkset's in a txt file, refer to "linkset.txt" as an example.

#### Usage:

```
[/path/of/src/files] $ rclink linkset.txt
[/path/of/src/files] $ rcunlink linkset.txt
```

### `steamrice`

Applies colors from a "theme.yaml" file to "\*.template" files in the directory.
I use it to change theme colors of my config files.
Refer to (dotfiles repo)[https://github.com/udiboy/dotfiles] for examples of "theme.yaml"
and template files.

#### Usage:

```
$ steamrice <-t|--theme theme.yaml> [-s|--source source-dir] [-d|--destination dest-dir] 
```

### `cpub`

A CLI epub reader written in pure python. Refer to it's README for details.

### `passwdmgr`

Password manager for the terminal. Equivalent would be GNU/pass, but I didn't want to mess around
with GPG keys and so many features.
It can store/retrieve/list/remove account+password stored in a file.
File is encrypted using AES-256 and stored as plaintext base64.

#### Usage:

```
Simple password manager for the terminal
usage: passwdmgr <command> [password-name]

Commands:
    create: Create new store file
    add: Add new password to the store
    get: Retrieve password from store
    rm: Remove password from store
    ls: List all stored passwords
    help: This text
Done!
```
