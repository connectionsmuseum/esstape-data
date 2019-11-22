# esstape-data
Data captured and decoded from the 3ESS generic tapes

This repository will host the following files for use with keleuk's "esstape" decoder:

* segments of audio that have been manually reconstructed
* decoded binaries
* readme files

* raw tape audio can be found here: https://drive.google.com/drive/folders/10Z6pookhHu3fHKLOJve7Mf0jtGPwTozj?usp=sharing

## Bin file format

Synchronization pre- and postamble are included

The files are stored bytewise big-endian. The tape is bitwise little-endian.

For example, the preamble, header, and first word of block `1/0001.bin`:

`8000 0801 33c0`

corresponds to a tape contents of:

`0000 0000 0000 0001   1000 0000 0001 0000   0000 0011 1100 1100`
