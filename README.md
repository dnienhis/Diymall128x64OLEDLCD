# Diymall128x64OLEDLCD
How I connected &amp; tested it

Initially I had some issues with this board - mainly due to some information I had (not sure where it came from) stating that the controller for this board was an SSD1306 device - so using the U8g2 Library I used the I2C constructor in the C demo code for the SSD1306 device and nothing seemed to work.

Fortunately my support request eventually landed with a lady named Jane at Shenzhen Flyfun Technology who got me straightened out.  Using the constructor for the SH1106 device in the U8g2 Library is all it took.  I compiled a few of the Demo's and everything seemed to play fine.  The Word Document has some screen shots etc. that may be helpful.

For the Text Output Demo's use this constructor:

U8X8_SH1106_128X64_NONAME_HW_I2C u8x8(/* reset=*/ U8X8_PIN_NONE);

For the Graphics Output Demo's use this constructor:

U8G2_SH1106_128X64_NONAME_1_HW_I2C u8g2(U8G2_R0, /* reset=*/ U8X8_PIN_NONE);

I attempted to make a video (BE KIND! LOL) and it's here:

https://youtu.be/OK1O9GoU9uc


