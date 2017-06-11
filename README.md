# DMXOPL
***
New and improved DMX GENMIDI for Doom and sourceports.


## Summary
This is a GENMIDI patch for DMX for OPL2-OPL3 FM synthesis. This patch aims to remedy the "weak" default instruments to better match the Roland Sound Canvas, most notably the SC-55 and SC-88. Recommended minimum setup for no note-cuts is  ZDoom 2.8.1 with MAME OPL2 emulator core, with 6 chips emulated.


# FAQ
***

### What did you use for this project?
Hex Editors, OPL3 Bank Editor, Fraggle's Python scripts, Adlib Tracker II, Edlib, ADLMidi. I also used the following keyboards and devices:

* Yamaha PSR-3 for basic percussion
* Yamaha PSS-50 for layered voice ideas
* Yamaha DX-7 
* Commodore 64 Music Module
* VRC7 and related chips
* Sound Blaster 16
* Yamaha PCI cards

### Will this run on Vanilla?
Yes, but some note cut-offs will happen if you don't have your **DMXOPTION** variables set. Even then, this may cut notes. I was aiming for sound quality with source ports that can run multiple OPL2/OPL3 chips, but I may release a cut-down version later.

### YOU MISSED (X) SOUND!
I've changed 99% of the sounds, but a few I liked enough to keep.

### What IWAD works best?
All IWADs work.

### Is this compatible with (X)?
As far as I know, anything that supports DMX patches would be supported. If you want this included in your favorite OPL plugins, please let the authors know. I would be more than happy to see this patch included.

### I'd like to use this in my project.
Go ahead, just give credit. My recommended string for plugins is "CSGOPL", "DMXOPL v1.7", or DMX(ConSiGno). DMX(Sneakernets) is also acceptable.

### How can I help?
Send a pull request.

# Credits
***
* Wohlstand, for the OPL3BankEditor
* Bisqwuit, for ADLMidi
* Fraggle, for Chocolate Doom and GENMIDI research, as well as the Python scripts
* SubZ3ro, for AdLib Tracker II
* Esselfortium, for the encouragement and support
* Jimmy, who will include this in the next Adventures of Square release
* The Fat Man, who created the famous 2-op and 4-op patches everyone knows
* Diode Milliampere, who made FM synth popular again
* Patchouli, for keeping my spirits up
* Graf Zahl, for continuing ZDoom as GZDoom
* Randi, for implementing the OPL Emulation in ZDoom
* Fisk, for miscellaneous feedback and MIDIs to test
* Stewboy, for the Ancient Aliens MIDIs to test
* Xaser, who said this patch passes the "Angry Scientist test"
* Minigunner, just because
* Altazimuth, who claims it'll be in Eternity someday
* MTrop
* Quasar, for Eternity Engine
* Glaice, for patch advice
* BlastFrog, for patch advice
* Vogons Forums, for the OPL-3 Research and tools
* AtariAge, for C64 Sound module preset banks
* NintendoAge
* John Chowning, the father of FM synthesis. I hope he can hear this someday.

## Extra Thanks to:
* Doomworld Forums and the IRC/DISCORD channels
* Giest118, who installed Doom again to listen to this
* Nuke.YKT, for testing this in Raptor, and for the Nuked OPL core
* kode54, who will add this to Foobar2K plugin and Cog
* Patch93, who inspired the new guitar patches
* Infurnus, for support
* Leileilol, for support

 YMF262 forever.