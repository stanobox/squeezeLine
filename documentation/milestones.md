

# squeezeLine milestones:

## raw list of ideas:

Given these [requirements](project_requirements.md), I can define the first few milestones here:

### dev environment:

#### IDE

* CLion
* Qtcreator
* C/C++ for Visual Studio Code
* vim ( not now, too early )
* other?

#### dev tool chain

* cmake
* make / autotools
* bash scripting

####  TDD / DDD

choose which framework to use (?)

#### UI:

I need to implement the timeline with tracks and clips

which toolkit is ok for this ?

* QT
* JUCE // this would be cool, since it provides "nearly" everything, and it's though for audio application from scratch.
* other (?)


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



