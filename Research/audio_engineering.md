### Informative [video](https://youtu.be/f9P7SeUlzQg) detailing a YouTuber's attempt to programatically noise reduce (June 2019)

- [SOX - Sound eXchange](http://sox.sourceforge.net/): command line audio engineering, last modified Feb 2015; noise reduction possible without the smoothing of Audacity
- [pydub](https://github.com/jiaaro/pydub): python package for audio manipulation, last modified Jul 2020; no noise reduction

### Audacity's Open Source noise reduction algorithm [file](https://github.com/audacity/audacity/blob/master/src/effects/NoiseRemoval.cpp) written in C++ (last edit May 2020)

> The first pass is done over just noise. For each windowed sample of the sound, we take a FFT and then statistics are tabulated for each frequency band - specifically the maximum level achieved by at least (n) sampling windows in a row, for various values of (n). 

> During the noise removal phase, we start by setting a gain control for each frequency band such that if the sound has exceeded the previously-determined threshold, the gain is set to 0, otherwise the gain is set lower (e.g. -18 dB), to suppress the noise. Then frequency-smoothing is applied so that a single frequency is never suppressed or boosted in isolation, and then time-smoothing is applied so that the gain for each frequency band moves slowly. Lookahead is employed; this effect is not designed for real-time but if it were, there would be a significant delay. 

> The gain controls are applied to the complex FFT of the signal, and then the inverse FFT is applied, followed by a Hann window; the output signal is then pieced together using overlap/add of half the window size.

