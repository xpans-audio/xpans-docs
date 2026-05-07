# xpans Spatial Record (XSR)

The xpans Spatial Record format is a data structure for serializing and
deserializing spatial properties. It contains the minimal amount of
information for reproducing a scene.

## Use case
XSR is not an ideal format for many cases. It is meant to be easily
read, written, and adapted in order to support the development of xpans
especially in the ecosystem's early stages.

## Data layout
XSR begins with the sample rate of the scene.

After that, it holds an array of spatial samples. In XSR, spatial samples only
need to be recorded if they are the first sample of the scene or any
audio source data has been changed since the previous sample.

Spatial samples contain the sample number and an array of 'events'.
Each event relates to only one audio source. An event contains the Source ID
the event is referring to, and the spatial properties that have changed since
the last sample.

Refer to XSR's 
[source code repository](https://github.com/xpans-audio/xpans_xsr)
for a more technical overview and a rough specification.
