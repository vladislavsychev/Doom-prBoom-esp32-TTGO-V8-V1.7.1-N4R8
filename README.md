DOOM prBoom mod for TTGO V8 v1.7.1 N4R8 with sdcard reader on board. Use ESP-idf 4.4. New one does not fly for that proj.

Have to use doom1.wad, doom2.wad, doom.wad, prboom.wad But sound alloc any case from doom2.wad. So your choise.
 
If want to use doom1 or doom2 just rename it to doom.wad and put altogether with prboom.wad in root of SDcard.
Some trick for SD card reading for TTGO v1.7.1 -
External pullup 10k to Pin2  and IT IS CRUTIAL> I dont know who is eng who made it shit but withouth external Pullup (5-10k) to io2 Sdcard reader on board does not work in SDmmc 1-bit mode. It also does not work in SD spi mode altogether with TFT spi anycase (st7789 or ILI9341) - off cause you can choise tye of TFT it in proj. But right now I build it for ST7789. 

TFT ST7789
(LCD pins   GPIO):
LCD_CS     io5,
LCD_CLK    io18,
LCD_MISO   io19,
LCD_RESET  io21,
LCD_DC     io22,
LCD_MOSI   io23

Current button mapping ( and you need pullup)
(GPIO    Action): 
sensor_vp      Move up, 
sensor_vn      Move down, 
io34           Move left, 
io35           Move right, 
io32           Use, 
io34           Fire

Sound DAC esp32 to ext amp. Whatever. 
Pin io25 or io26. Mix problem io25 right, io26 left.
