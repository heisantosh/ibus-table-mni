# mni-mayek

# :earth_asia: 

IBus input table for Manipuri language using Meetei Mayek script.

## Mappings

| Mayek | Keys | Mayek | Keys | Mayek | Keys |
|:-----:|:----:|:-----:|:----:|:-----:|:----:|
| ꯀ      | k    | ꯛ     | K    |  ꯣ      | o   |
| ꯁ      | s    |       |      |  ꯤ     | i   |
| ꯂ      | l    | ꯜ     | L     |  ꯥ     | a   |
| ꯃ      | m    | ꯝ     | M     | ꯦ     | e   |
| ꯄ      | p    | ꯞ     | P     |  ꯨ     | u   |
| ꯅ      | n    | ꯟ     | N     | ꯩ     |  ou  |
| ꯆ      | ch   |      |       | ꯪ     | ngg  |
| ꯇ      | t    | ꯠ     | T     | ꯫    | CH   |
| ꯈ      | kh   |      |       |   ꯭    | APUN  |
| ꯉ      | ng   | ꯡ     | NG    | ꯬     | LUM |
| ꯊ      | th   |      |       | ꯰    |  0   |
| ꯋ      | w    |      |       | ꯱    |  1   |
| ꯌ      | y    |      |       | ꯲    |  2   |
| ꯍ      | h    |      |       | ꯳    |  3   |
| ꯎ      | uu   |      |       | ꯴    |  4   |
| ꯏ      | ee   | ꯢ     | EE    | ꯵   | 5    |
| ꯐ      | f    |      |       | ꯶    |  6   |
| ꯑ      | aa   |      |       | ꯷    |   7   |
| ꯒ      | g    |      |       | ꯸    |    8  |
| ꯓ      | z    |      |       | ꯹    |    9  |
| ꯔ      | r    |      |       |     |     |
| ꯕ      | b    |      |       |     |     |
| ꯖ      | j    |      |       |     |     |
| ꯗ      | gh   |      |       |     |     |
| ꯘ      | dh   |      |       |     |     |
| ꯚ      | v    |      |       |     |     |


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

# TODOS

* Update mappings to include Unicode extensions
* Package for Ubuntu
