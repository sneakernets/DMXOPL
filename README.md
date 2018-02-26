# DMXOPL3
***
New and improved DMX GENMIDI for Doom and sourceports, taking full advantage of the OPL3 waveforms. This takes things up a notch in terms of timbre.


## Summary
This is a GENMIDI patch for DMX for OPL3 FM synthesis. This patch aims to remedy the "weak" default instruments to better match the Roland Sound Canvas, most notably the SC-55 and SC-88. Recommended minimum setup for no note-cuts is ZDoom 2.8.1 with DOSBOX OPL3 emulator core, with 6 chips emulated.

## How To Use in DOOM (Vanilla, DOS)
**NOTE:** I'm assuming you use a Sound Blaster Pro 2, or SB16/AWE32/AWE64. The original Sound Blaster Pro won't work!
1. Download `GENMIDI - Vanilla.op2`, rename it to `GENMIDI.op2`, and put that in your doom directory. *Do not name it anything else!!*
2. Set up and save a batch file like this:
   ```batch
   @ECHO OFF
   SET DMXOPTION=-opl3
   doom -file GENMIDI.op2
   PAUSE
   ```
   Feel free to add any additional files like PWADs if you want. It's just a file, after all.
3. In `SETUP.EXE`, make sure the correct Sound Blaster is selected for your music card. I've been told Pro Audio Spectrum also works if    OPL3 can't be detected properly.
4. Run your batch file. That's it!

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
Yes, but your **DMXOPTION** variables must be set. There also may be note cuts on certain music selections, although this is very rare in the IWADs.

### YOU MISSED (X) SOUND!
Pretty much every single sound has been replaced at this point. If there are any that haven't been changed, it's likely due to me not getting around to it, or not knowing about it. Since GENMIDI is a binary format, getting diffs on it is a pain, so I don't know which instruments are changed and what isn't. If you know a way to check for this, let me know!

### What IWAD works best?
All IWADs work.

### Is this compatible with (X)?
As far as I know, anything that supports DMX patches and OPL3 emulation would be supported. If you want this included in your favorite OPL3 plugins, please let the authors know. I would be more than happy to see this patch included.

### Will any instruments use 4-op?
In the OPL3 sense, No, at least for GM sounds. XG and GS sounds (WOPL only) may be a different story. We'll just have to see.

### Why not just use a soundfont?
Because all soundfonts I've heard *stink* compared to the SC55, and to this day i'm not satisfied with the state of Sound Canvas soundfonts, or the software midi sequencers that claim to use them.

### Something doesn't sound quite right.
All DMX implementations seem to differ from port to port and player to player. My patches are tested in Vanilla Doom, Chocolate Doom, and ZDoom 2.8.1. If you hear something different that you don't hear in those three ports, it is a bug that should be reported to the respective authors. However, some sounds may sound louder than others. This is due to the way DMX handles velocity on voices with maxed out volume, which has largely been addressed by now.

### I'd like to use this in my project.
Go ahead, just give credit. My recommended string for plugins is "DMXOPL3", or "DMXOPL3 v2.x". "DMXOPL3 by Sneakernets" is also acceptable. Also, don't erase the original DMXOPL preset for this one - I'd love to see both included if possible!

### How can I help?
Send a pull request. Submit your instrument as a OPLI format instrument in the "Contributions" directory.

# WOPL FAQ

### What's the difference between the WOPL version and the DMX version?
The main difference is with a few instruments that had to be tweaked to work with DMX. Most of these changes are negligible for General MIDI stuff. To hear what I intended DMXOPL to sound like in Doom, you'll have to wait for Eternity Engine's ADLMIDI support to be finalized.

### Any plans for GS/XG support?
Yes. This will take considerable time, and voices will be added as I come across them in my MIDI files. You can check the progress on those through the XG and GS branches that I will make (or have already made). As I think the GM set is solid enough now, save for just a handful of instruments, I can start work on the other banks.

### Will the WOPL version be usable on any other FM chips?
Depends on the chip, but more than likely the answer is *no*. YMF262 (and the OPL* family for that matter) operate differently than most of the other FM chips, and wouldn't likely transfer over to DX-7 or other instruments without considerable work, if they would work at all.

### Is the best way to listen to this *really* through an emulator?
Yes, unfortunately. Unless someone makes an FM chip that can handle 128+ channels, this is likely never to change. If you're using this in your music projects and you *still* want to use the real thing, I recommend recording one track at a time and throwing the result in your favorite DAW - just be sure to put a highpass filter set to a really low value (I recommend 5 Hz) to get rid of the offset garbage, lest your mix splatter like crazy.

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
* Altazimuth, who claims it'll be in Eternity someday (this is now true)
* MTrop
* Quasar, for Eternity Engine
* Glaice, for patch advice
* BlastFrog, for patch advice
* Vogons Forums, for the OPL-3 Research and tools
* AtariAge, for C64 Sound module preset banks
* NintendoAge
* John Chowning, the father of FM synthesis. I hope he can hear this someday.

## Extra Thanks to:
* Doomworld Forums and the respective IRC/DISCORD channels
* The 4th Modulator DISCORD channels
* Giest118, who installed Doom again to listen to this
* Nuke.YKT, for testing this in Raptor, and for the Nuked OPL core
* kode54, who added this to Cog and FB2K, thank you!
* Patch93, who contributed various patches
* OlPainless, who contributed various patches
* Papiezak, who contributed various of patches
* Infurnus, for support
* Leileilol, for support
* MaliceX, for support
* Kuschelmonster, for support
* Anyone who makes music with this thing!

 YMF262 forever.
