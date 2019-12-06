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

* Requires
    * [Coreutils](https://www.gnu.org/software/coreutils)
    * [Apt-get](https://salsa.debian.org/apt-team/apt)

* Installation

    ```bash
    git clone https://github.com/zakariagatter/apt-undo ~/apt-undo
    mkdir -p ~/.local/bin
    cp ~/apt-undo/bin/apt-undo ~/.local/bin
    chmod +x ~/.local/bin/apt-undo
    ```

## Help
```
Apt-undo Undo Apt-get action
apt-undo OPTIONS ACTIONS PKG ...

OPTIONS
 -u | --undo <pkg>  : Undo action with pkg in it
 -c | --count <num> : Undo last Number of actions
 -h | --help        : SHow help dialog

ACTIONS
 install : any use of apt-get install
 remove  : any use of apt-get remove
 purge   : any use of apt-get purge
```

[Apt-undo]:https://github.com/zakariagatter/apt-undo
