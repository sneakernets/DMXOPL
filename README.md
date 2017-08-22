# DMXOPL3
***
New and improved DMX GENMIDI for Doom and sourceports, taking full advantage of the OPL3 waveforms. This takes things up a notch in terms of timbre.


## Summary
This is a GENMIDI patch for DMX for OPL3 FM synthesis. This patch aims to remedy the "weak" default instruments to better match the Roland Sound Canvas, most notably the SC-55 and SC-88. Recommended minimum setup for no note-cuts is  ZDoom 2.8.1 with DOSBOX OPL3 emulator core, with 6 chips emulated.


# FAQ
***

### Why OPL3 only?
OPL3 has four additional waveforms - Alternating Sine, Camel Sine, Square, and Logarithmic Square (Sawtooth). The most interesting of these is the Square wave, for obvious reasons! This will benefit percussion instruments immensely.

### What did you use for this project?
Hex Editors, OPL3 Bank Editor, Fraggle's Python scripts, Adlib Tracker II, Edlib, ADLMidi. I also used the following keyboards and devices:

* Yamaha PSR-3 for basic voice ideas
* Yamaha PSS-50 for layered voice ideas
* Yamaha DX-7 
* Commodore 64 Music Module
* VRC7 and related chips
* Sound Blaster 16
* Yamaha PCI cards
* Sounds from various SEGA MegaDrive games


### Will this run on Vanilla?
Yes, but your **DMXOPTION** variables must be set.

### YOU MISSED (X) SOUND!
Only gunshot is the same. Sorry, kid!

### What IWAD works best?
All IWADs work.

### Is this compatible with (X)?
As far as I know, anything that supports DMX patches and OPL3 emulation would be supported. If you want this included in your favorite OPL3 plugins, please let the authors know. I would be more than happy to see this patch included.

### Will any instruments use 4-op?
In the OPL3 sense, No.

### Why not just use a soundfont?
Because all soundfonts I've heard *stink* compared to the SC55, and to this day i'm not satisfied with the state of Sound Canvas soundfonts, or the software midi sequencers that claim to use them.

### Something doesn't sound quite right.
All DMX implementations seem to differ from port to port and player to player. My patches are tested in Vanilla Doom, Chocolate Doom, and ZDoom 2.8.1. If you hear something different that you don't hear in those three ports, it is a bug that should be reported to the respective authors.

### I'd like to use this in my project.
Go ahead, just give credit. My recommended string for plugins is "DMXOPL3", or "DMXOPL3 v2.0". DMXOPL3(Sneakernets) is also acceptable. Also, don't erase the original DMXOPL preset for this one - I'd love to see both included if possible!

### How can I help?
Send a pull request. Contributing is easy, just follow the guide.

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
