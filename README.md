# Sam_Coupe_1bit_Music
Sam Coupe 1bit Music - ported from ZX Spectrum.


UTZ & Shiru's 1bit music from the ZX Spectrum ported to the Sam Coupe computer, intiially as a work-in-progress and a test to see if it can actually be done.
Note that the speccy and a number of other Z80's typically run around the 3.5 mhz mark. The Sam Coupe runs at 6Mhz, so timing is all off, and most (all) of these 1-bit pieces of music all sound 'out-of-whack'. Some engines implement an external speed control to that of the actual music date, whilst otehrs have the speed implemented within the music bytes themselves.  So - some can be adjusted and others is somewhat near impossible to change for the likes of my dumb self.

   Sam Coupe uses Ports 511 & 255 for AY music, whilst it uses bit 4 on port 254 ($FE) for its direct speaker/beeper access (exact same as ZX speccy).
   
   Assembly origin is typically $8000.

   Nothing else is required; no fancy headers required.  Directly assemble any of the ZX's asm code to $8000, place on to a disk image, load the disk image, run the load command and listen.


1. Assemble the 1-bit music straight to a binary - as a standard ZX spectrum binary.  Depending on the asm code, most will assemble with either SJASMPLUS (Shiru's preferred assembler) or PASMO (Utz's typical preferred assembler). SJASMPLUS can be found on Github. Pasmo can be found via google search on some little-known ZX website.

2. Use a disk manager to create a disk image, and add the binary.  eg: "Andrew Collier's SimCoupe .DSK manipulator" utility. Write the assembled music binary (MUSIC.BIN)  to the disk image. Write the disk image to a disk file (MUSIC.DSK).

3. Load the disk into the likes of SimCoupe emulator or equivalent. Do a DIR.

4. Run this command to load the music binary from the disk image :         LOAD "music.bin" CODE 32768

5. Listen to the bad timing, but !working!, 1bit beeper tunes from your Sam Coupe emulator or real hardware.

Dave - Oct 2024.


   
