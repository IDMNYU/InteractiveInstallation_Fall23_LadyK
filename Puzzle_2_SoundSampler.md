# Interactive Installation 

* **DM-GY 4913-B Special Topics: Interactive Installation**

## Puzzle 2: Create a Max patch that is a sound player and mixer/sampler. It needs to output a 90 second audio piece that is random in it's composition.

In order to do this, we need to have several sound files that load into your patch (or automatically load into it). One needs to be able to manipulate and fracture these sounds to smaller loops. We need the ability to save these loops, not to mention to output these loops so that we can hear them, along with volume manipulation.

##### Playing sounds: 

* _groove_ object plays a sound file that's played from a _buffer_. Make sure to check out the help file, as well as all of the input messages and objects to control it. With the _groove_ object, you can control pitch (via the _sig~_ object), which affords many many options for new sounds.

* _sfplay_ object also plays a sound file, yet not from a buffer. Make sure to check out the help file, as to how to control it with what sound file is playing, looping and playing between certain points in the sound file.

##### Recording settings:

* _preset_ object. Make sure to understand how to record settings, and to play those settings.


##### Outputing your audio to the sound output on your laptop:

* _dac_ object will afford you much more in the long run than the...

* _ezdac_ object

##### Volume control

* _* ~_ object + _line~_ object. Here, you can send floats to the line, and control the level of audio on the fly

##### Random composition

* _urn_ object won't repeat numerical selections

* _decide_ object can choose randomly between 2 values

* _scale_ object can output a value within a range, based on a random input


##### Selecting files, file manipulation

* _dropfile_ object creates a field where files can manually drop in

* _opendialog fold_ object to get a directory path to a file

* _folder_ object can load all the files in a folder of a particular formate type. (check it out with the umenu object).


##### other nice helpful objects to check out to facilate the above and more:

* _umenu_ object

* _trigger_ object

* _gate_ object

##### Timing sounds and the composition

* this builds off all the objects from the poem patch

* the _counter_ object + the _metro_ object can keep track of how long your patch has been running. 

* _sfplay_ will bang when done playing a sound file. Otherwise with _groove_ you'll need to time the length of the audio file to create a secondary timer to bang upon file completion.

Your patch should play more than one sound file at a time, at times, during your composition. After getting an initial patch working, you need to explore your sound files to _find_ new sounds within those sounds. Save those to your preset object to recall later. 

Then, coreography the entry and exit of each of these sound bites, as well as how often they appear, and as to when they appear. Play with volume to add layers and textures

When your patch is loaded and a bang is sent, a 90 second layered audio piece of unknown composition will play for your viewers.

See also:
* MSP  Basics tutorial: 1: Test Tone
* MSP  Basics tutorial: 2: Ajustable Oscillator
* MSP Sampling Tutorial 1: Recording and Playback
* MSP Sampling tutorial 2: Play back from Multiple Sample Points
* MSP Sampling tutorial 3: Playback with Loops
* MSP Sampling Tutorial 6: Record and Play audio files
* Max tutorial 19: Timing

* submit your patch to your github repo label as FirstName_P2.maxpat