# Sam_Coupe_1bit_Music
Sam Coupe 1bit Music - ported from ZX Spectrum.


UTZ & Shiru's 1bit music from the ZX Spectrum ported to the Sam Coupe computer, intiially as a work-in-progress and a test to see if it can actually be done.

1. Assemble the 1-bit music straight to a binary - as a standard ZX spectrum binary.

2. Use the DSKMAN.EXE Sam Coupe disk manager program to create a new disk and to write the binary to the disk.

3. load the disk into the likes of SimCoupe emulator. Do a DIR.

4. LOAD "file.bin" CODE 32768

5. Listen to the bad timing, but !working!, 1bit beeper tunes from your Sam Coupe emulator or real hardware.



   Sam Coupe uses Ports 511 & 255 for AY music, whilst it uses bit 4 on port 254 ($FE) for its direct speaker/beeper access (same as ZX speccy).
   Assembly origin is typically $8000.

   
