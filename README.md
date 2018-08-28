# mni-mayek

IBus input table for Manipuri language using Meetei Mayek script.

# Custom install instructions

Tested on Ubuntu 18.04.1 LTS "Bionic Beaver"

Follow the instructions on the IBus github wiki at [https://github.com/ibus/ibus/wiki/HowToCreateATableForIBusTable](https://github.com/ibus/ibus/wiki/HowToCreateATableForIBusTable).


## Install the data
```bash
$ DATA_DIR=/usr/share
$ sudo ibus-table-createdb -n ${DATADIR}/ibus-table/tables/mni-mayek.db -s mni-mayek.txt
$ sudo cp mni-mayek.svg ${DATADIR}/ibus-table/icons/ 
$ # Restart IBus
$ ibus-daemon -drx
```

## Add input method

1. Select: Settings -> Region & Language -> Input Sources
2. Click on `+` to add an input source
3. Select: Other -> Manipuri(Manipuri)

## Start typing

Use `Super` + `Space` to switch between the input sources.

NB: Not all applications support input using IBus.

# Package

TODO: Create package for Ubuntu