DOOM prBoom mod for TTGO V8 v1.7.1 N4R8 with sdcard reader on board. Use ESP-idf 4.4. New one does not fly for that proj.

Have to use doom1.wad, doom2.wad, prboom.wad But sound alloc any case from doom2.wad. So your choise.
 
Just rename doom1.wad or doom2 to doom.wad and put altogether with prboom.wad in root of SDcard.
Some trick for SD card reading -
External pullup 10k to Pin2

TFT ST7789
(LCD pins   GPIO):
LCD_CS     io5,
LCD_CLK    io18,
LCD_MISO   io19,
LCD_RESET  io21,
LCD_DC     io22,
LCD_MOSI   io23

Current button mapping
(GPIO    Action): 
36      Move up, 
34      Move down, 
32      Move left, 
39      Move right, 
33      Use, 
35      Fire

Sound DAC esp32 to ext amp. Whatever. Does not check at all.
Pin io25 or io26. Mix problem io25 right, io26 left.
