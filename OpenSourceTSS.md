# Open Source TTS

## Platforms to support

* macOS
* Linux
* Windows (does most likely require an API license from MS)
* Android
* iOS

## Text processing & conversion to synthesis symbols

Text processing is done using Hfst and VislCG3 through the
[libdivvun](https://github.com/divvun/libdivvun). It is assumed for the purposes
of this tender that the text processing is developed and done by the Divvun
group.


* new libdivvun module must be developed for pipeline integration of the
  speech synthesis engine

## Speech synthesis engine

* must be open source
* a possible candidate is the [festival system](http://festvox.org/)
* another candidate is [Idlak](https://github.com/idlak/idlak)
* other open-source engines may be suggested
* the selection of engine must be done in cooperation with Divvun and its
  partners, as the engine used for synthesis must be the same as or compatible
  with the one used for voice generation.

* proper integration with the different operating systems
    * closed-source integration will be accepted if required by the OS wendor
