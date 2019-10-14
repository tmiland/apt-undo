# apt-undo

## About
[Apt-undo] undo the last apt-get action

[Apt-undo] allows you to ...

* View all packages Install with giving PKG in giving ACTION
* Undo the ACTION that have PKG in it
* Undo N Last ACTIONS Times

[Apt-undo] automatically ...

* check for giving ACTION
* check for giving PKG

## Set Up

* __Installation__ :

    ```bash
    git clone https://gitlab.com/zakariagatter/apt-undo
    cd apt-undo
    mkdir -p ~/.local/bin
    cp apt-undo ~/.local/bin
    chmod +x ~/.local/bin/apt-undo
    ```

## Help
```
APT-UNDO : undo the last apt-get action
    Write by ZAKARIA GATTER (https://gitlab.com/zakariagatter)

    apt-undo [OPTION] [ACTION] PKGS ...

    OPTIONS :
       -w | --with [ACTION] PKGS : Display all the packages been with PKGS in the ACTION
       -u | --undo [ACTION] PKGS : Undo the [ACTION] that have PKGS in it
       -c | --count [ACTION] [N] : Undo the last [ACTION] for [Number] of Last actions
       -h | --help               : This Help Dialog

    ACTIONS :
        Install : The Install action like 'sudo apt install'  or any similar command
        Remove  : The Remove action  like 'sudo apt remove'   or any similar command
        Purge   : The Purge action   like 'sudo apt purge'    or any similar command

    NOTE :
        if you leave [N] Empty, apt-undo take '1' as the default value
        Apt-undo Process One package or Action at a time is much easier and more manageable
```
[Apt-undo]:https://gitlab.com/zakariagatter/apt-undo
