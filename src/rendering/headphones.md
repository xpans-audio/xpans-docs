# Headphones

## Maximum ITD
The maximum amount of time an audio source will be delayed in the ear farthest
from the source. The ear closest to the source always experiences zero delay.

Maximum ITD is typically represented in nanoseconds or microseconds. It
should never exceed 1 millisecond for practical renders.

## Distance
Distance cues are rendered by reducing the interaural level difference (ILD) as
distance increases. This effect relies on interaural time difference (ITD) to
preserve the listener's localization of the source. Without ITD, this effect
can cause the listener to incorrectly localize the direction of audio sources.
Distance does not affect interaural time difference (ITD).

### Distance curve

#### Linear
Applies a linear curve to the normalized distance.

#### Exponential
Applies an exponential curve to the normalized distance.

### Minimum distance
The distance from the listener where an audio source will sound closest.

### Maximum distance
The distance from the listener where an audio source will sound farthest.

### Distance effect
The distance effect parameter scales the amount that the ILD will be reduced
based on distance. When distance effect is `1.0`, the ILD will be reduced to
zero when a source is greater than or equal to the maximum distance. When
distance effect is zero, the ILD will never be reduced regardless of a source’s
distance. It is not recommended to set the distance effect to a high value as
it may make it hard for listeners to localize frequencies above 1,500 Hz.

## Pan laws
The following pan laws are implemented:
- -3dB with sine taper
- -3dB with square root taper
- -6dB with linear taper
