
### define a dev environment:

My inexperience in the C++ world force me to go really slow, step by step. \
**Every concept below will be subject to changes**.



#### UI framework:

This choice will drive the whole dev env setup, mainly.

Need to implement the timeline with tracks and clips...\
which toolkit is ok for this ?

**Juce** ( well documented ) // this would be cool, since it provides "nearly" everything, and it's though for audio application from scratch.\
**Nuklear** ( beign "Immediate Mode" forces me to learn more... )\
**Qt** ( personally I'm a bit skeptical about this, being it really heavy )\

On top of that, it could be nice to use **GuiLite within another framework** ( Juce or Qt, mainly )



#### IDE:

The final decision, actually, is left to the developer, obviously.\
I was given some suggestion, so the choice for the IDE will be made between:
* **CLion**
* **Qtcreator**

These were discarded:
* C/C++ for Visual Studio Code // for no particular reason
* vim // too "bare metal" to start learning C++



#### Build systems:

the choice will be probably
* **cmake**

These were discarded:
* make / autotools // I love the idea, but probably I can go back to them in another project
* bash scripting // would be cool and would be, honestly, a time sucker, too.
* qmake // I perfer to not tie the build system to a specific framework. Afaik, this is mainly used beside Qt framework.


####  TDD / DDD framework:

I'm looking around. I will probably use one of these:

* Catch
* Google Test

( Quite sure I'm gonna use **Google Mock** for mocking )



## Draft for next steps...

```text

### get precise timing impulse, to trigger events

what option do I have ?
are the ones below available?

* ALSA sequencer/raw MIDI API
* kernel syscall
* a "simple thread" with a callback function
    
do I need "real time preemption" ?

_i.e. do I need rlimits() and such ?_


### UI: how implement the timeline ( with clips )
     
what are the designs pattern useful for this ?

         
### I/O:
    
* how to read from GPIO
* how to read/write to ALSA USB/MIDI
* how to do all that from user space

```
