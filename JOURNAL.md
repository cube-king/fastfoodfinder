# 5/25/2025
Today, I worked on the basic idea as well as finding compatible components. Through a few google searches (and past experience), I came across the "XIAO ESP32S3"! Boasting a total of 11 GPIO pins (just right for my use case) and WIFI / Bluetooth capabilities, it seems perfect for the job. I was able to import the symbol and footprint through the XIAO OPL library quite easily, and began routing up the NeoPixel ring to it! I've decided to integrate my own 16 NeoPixel version of a NeoPixel ring into the PCB, allowing for on-board control and easy soldering! 

The exact details of the PCB I'll worry about later - for now I just want to get all components wired up on the schematic for easy access later. I did attempt to arrange NeoPixels in a circular shape on the PCB, but it seemed finnicky and hard to deal with, so we'll cross that bridge when we come to it. I was successfully able to connect several components to the ESP32, but that's beside the point. I'll also be using a GPS unit and magnetometer to determine position and direction, so let's find the ideal models and footprints of those quickly.

From a quick google search, we can find that the NEO-6M GPS module seems to be the most compatible with the average ESP32 devboard, and it communicates with the board through the TX and RX pins. There are many available tutorials and guides online for ESP32 compatibility with the NEO-6M, so this is what I'll be using for my device! I was able to find a footprint [here](https://easyeda.com/components/NEO-6M-V2-GPSMODULE-FOOTPRINT_3058736435b7485c9cb912d26a86a5a2), but it was an EasyEDA file which I'll convert tomorrow. A promising lead seems to be the uPesy/easyeda2kicad repository, which demostrates a method to convert a footprint file from EasyEDA to a KiCad file using Python! 

 ![Current setup](https://hc-cdn.hel1.your-objectstorage.com/s/v3/41e41e053c133dbe3e31a589573f20627973fca1_image.png)
 (Current setup as of 5/25/25)

As of 5/25/25, I've spent at least 3 hours fiddling with various parts of the project and researching. 

Tomorrow, I'll work on finishing the schematic (by adding the remaining components: magnetometer, GPS module, OLED display, 5 buttons) and configuring the PCB. The next day (that I can work), I'll make some mockup software and add finishing touches to the PCB. Finally, it'll be time to submit the project, and cobble together my FastFoodFinder compass!

---
# 5/26/2025
