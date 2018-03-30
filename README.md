Q2K Key Map parSer
ver. 0.0.69 (who knows)
by 2Cas (c) 2018
MIT licens

For parsing keymaps from QMK Firmware style keymap.c files to Keyplus YAML format

Requires: Python3.4 pyyaml pyparsing
avr-gcc

Run with:
python3 prepr.py [KEYBOARD NAME] [CMD LINE OPTIONS]

For example:
python3 prepr.py clueboard/66 -r rev2


Run python3 prepr.py -h for cmd line options

####
Usage: python3 prepr.py [KEYBOARD] [-h] [-m keymap] [-r ver] [-L] [-M] [-R] [-S string] [-c keymap] 

positional arguments:
  KEYBOARD    The name of the keyboard whose keymap you wish to convert

optional arguments:
  -h, --help  show this help message and exit
  -m keymap   The keymap folder to reference - default is /default/
  -r ver      Revision of layout - default is n/a
  -L          List all valid KEYBOARD inputs
  -M          List all valid KEYMAPS for the current keyboard
  -R          List all valid REVISIONS for the current keyboard
  -S string   Search valid KEYBOARD inputs
  -c keymap   Select keymap template index
#####

VERY alpha, not every keyboard is gaurenteed to work 100%. Lots of uncaught exceptions will be thrown