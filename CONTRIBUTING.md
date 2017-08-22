# Contributing

Would you like to help with DMXOPL? Great! Here are some tips on contributing!

## Overall Rules

Here are a few general things to note:

* I may not accept all submissions.
* If I accept your submission, you will get credit.
* If I tweak your submission, you still get credit for it.
* If you submit just a rip from a game, I'm not going to accept it. The goal isn't to mix-and-match patches from various games, but to create new ones, or use existing ones as a base for your own derivative work.

## Guidelines

### Make sure your patch works on the 88-key range of a piano.

Not doing so will cause certain musics to sound quite terribly. The main reason for this is that some midi files used ranges outside of "normal" for some patches, Ex: a very high slap bass note.

### Make sure the volume of your patch matches the rest of the voices.

This may seem like a hard task, but all you need to do is take a MIDI file you know quite well, play it with your patches, and adjust the carrier volume accordingly. If you make a doublevoice patch and the result is too loud, turn the carriers down to 55 and work from there.

### Avoid large negative detuning numbers.

Some patches do use negative values, but if your patch needs a lot of detuning, please use the positive range, not the negative. For instance, a 10 detune patch will work, but a -10 detune won't work. The reason for this is that some DMX implementations cannot handle negative detuning past a certain limit and will play wrong notes entirely. Most of this depends on implementation of the player or the CPU arch the player is running on, but we need to support as many implementations as possible, including Vanilla DMX.

### Avoid "Fat Man" timbres.

Basically this means "Don't let your patches sound like Windows MIDI Mapper with a Sound Blaster Pro". While Fat Man's 2-op set was used *a lot* in the videogame industry, that doesn't mean it's a good idea to use. People are *tired* of hearing these timbres.

### Make sure your patch matches pitch of every other patch.

If you are making a guitar or bass patch, please make sure the result's octave ranges match the rest. A failure to do so will make your patch "stand out" and sound incorrect (because it is).

### Don't be afraid to "fake" resonance with double voice.

DMXOPL is no stranger to this : French horn patch uses a detune technique to get the iconic resonance of a French Horn.

### Check all methods of attack for any odd sounds.

This scenario is all too common: You think you have a great cymbal patch, and then someone makes a midi that expects the cymbal to resonate with a very short note, and your patch breaks. This happened to me more than once. For Crash Cymbals and chordophone percussion, always have attack set to 15.

### Don't rely on feedback too much.

Feedback can ruin a sound at quiet volumes, and the sound your'e looking for is most likely available using traditional methods.

### Make sure your patch doesn't crackle, beat with distortion, or sound too robotic.

Pulse-Sine has a lot of trouble with certain frequencies, so avoid using it if possible. It can create a "beating" effect that isn't very pleasant. Using Vibrato on certain modulator volumes can also exhibit this beating noise.

## Bugs

* Low Bass notes, if detuned in the negative range, may break.
* Certain DMX implementations play fixed percussion notes an octave lower or higher than normal.

----
Have fun!
