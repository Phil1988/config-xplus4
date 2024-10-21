# X Plus 4 config files

WIP and very much under construction, do not install on your printer without ability to revert.

if you want to test, in the meantime, copy this and paste it into ssh on the printer:
```
cd /home/mks/printer_data/config/ && git clone https://github.com/qidi-community/config-xplus4 && sed -i '/<---------------------- SAVE_CONFIG ---------------------->/i [include config-xplus4/*.cfg]' printer.cfg
```
then do a firmware restart.

if you already installed, the current update procedure is pasting and running this line: 
```
cd /home/mks/printer_data/config/config-xplus4 && git reset main --hard && git pull
```
then do a firmware restart. Beware that if you had done any modifications to the mods stored in the `config-xplus4` folder, they'd be erased by this action. 
