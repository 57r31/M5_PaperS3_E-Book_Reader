# M5Stack PaperS3: E-Book reader
This is a very simple prototype E-Book reader for the M5Stack PaperS3.
https://docs.m5stack.com/en/core/paperS3

It comes with a small sample of the start of Robopocalypse as a test. It's worth a read, it's a good book.       
If you like it, please support the author and buy the full book.                 
https://en.wikipedia.org/wiki/Robopocalypse                 
https://www.amazon.com/dp/B007YATMOE/                   
https://www.amazon.co.uk/Robopocalypse-Contemporaries-Daniel-H-Wilson-ebook                      

This E-Book/E-Reader a **prototype** so please note, it's very limited, for instance:           
1. Uses only 1 font.
2. Loads a single book "book.txt" from the root of your SD card.
3. Pages don't always exactly end in the same place at the bottom of the screen.

**Features_____**                   
1. Navigation by the jog wheel.                
Left: Previous page.           
Right: Next page.               
Push (hold for 4 seconds): On / Off                
(The Paper shows "Off" at the bottom center of the screen when it's off, but still displays the current page. No "Off" screen yet. =)  )
2. Remembers your page in the book for when you power back up.
3. Fast page drawing.
4. Date/Time and "page of pages" bar at the bottom.

I've also coded it to be accessible to all devs - I've not split it out into classes or used much in the way of dynamic allocation or pointer/reference useage, it's just a single familiar Arduino .ino file. It's quite short too. That means adding features like touch navigation, SD card browsing, font changing - can all be experimented with, while avoiding plunging headlong into polymorphism, encapsulation, multiple inheritence, abstract classes, pure virutal functions, advanced data abstraction, templates and so on. (yikes!)

**Features for the future:______**
1. A Micro SD card browser to select the book you want to read.
2. A font changing option. Just remember the startIndex of the page, then re-parse the book page start/stop positions in the new font size, make a note of the page that coincides where startIndex is, and display that page. 
3: A screen tap navigation option, to type the page number to go to.
4: WiFi book upload/download. Reading place synchronisation between M5 PaperS3.
5: Support for Mobi, EPub... etc....
6: Support for images, and page covers.

