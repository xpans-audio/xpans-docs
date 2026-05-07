# Mono

Mono rendering ignores all audio sources' spatial data and sums the scene's
audio channels together into one, optionally copying the resulting audio
channel to several more.

## Channel Count
The channel count parameter controls how many channels the mono rendering
will output. When set to `1`, only one channel will be output. When set to `2`
or higher, the sum of all sources' audio signals will be output to that number
of channels with each output channel containing identical audio data.
