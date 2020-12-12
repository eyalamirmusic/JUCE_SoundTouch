# JUCE_SoundTouch

A JUCE module that wraps the SoundTouch library in a JUCE-style module.

https://github.com/juce-framework/JUCE
https://gitlab.com/soundtouch/soundtouch

To use, clone and copy the ea_soundtouch folder into your project somewhere.

If using the Projucer, go to the modules section of your project, click the "+" button and choose "Add a module
from a specified folder".

If using CMake, use:
```cmake
juce_add_module(ea_soundtouch)
```
and then in your code:
```cpp
#include <ea_soundtouch/ea_soundtouch.h>
```

(When using the Projucer, this include is automatically generated)


Background:
------------

The work here was inspired by a similar wrapper done by the tracktion_engine (an incredible code base, BTW!)
https://github.com/Tracktion/tracktion_engine

Their wrapper is great, but it only works if you bring the entire engine as a dependency, so I tried creating a lightweight
version that requires no additional dependencies.

License:
--------

Using my (very small) chunk of code is totally free for every personal or commercial reason.
However, please check the license for both JUCE and SoundTouch.
