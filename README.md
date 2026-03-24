DOOM prBoom mod for TTGO V8 v1.7.1 N4R8 with sdcard reader on board

use doom1.wad, doom2.wad prboom.wad
rename doom1.wad or doom2 to doom.wad
Trick for SD card reading
External pullup 10k to Pin2

TFT ST7789
LCD pins   GPIO
LCD CS     io5
LCD CLK    io18
LCD MISO   io19
LCD RESET  io21
LCD DC     io22
LCD MOSI   io23

Current button mapping:
GPIO    Action 
36      Move up 
34      Move down 
32      Move left 
39      Move right 
33      Use 
35      Fire

Sound DAC esp32 to ext amp. Whatever. Does not check at all.
Pin io25
