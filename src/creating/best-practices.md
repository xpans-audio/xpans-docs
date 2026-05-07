# Best Practices

## Maintaining signal separation
In xpans, each audio signal or 'voice' is meant to exist in only one audio
source. When an audio signal is shared between two or more audio sources
(aka signal sharing), it can be subject to phase interference in rendering 
modes that use delay to create or enhance spatial impression (i.e.
headphones).

This can be unpleasant for listeners and can make your mix extraordinarily
difficult to quality control. It is okay to combine multiple audio signals
into one audio source, but you must ensure no audio signals are shared by
two or more audio sources.

> Note: If you would like to intentionally break this rule for creative
> experimentation, make sure you are monitoring your mix in as many formats as
> possible to ensure your intention is preserved.

### Panning across audio sources

Panning across audio sources inherently involves signal sharing.
It's best to leave channel-based panning to the renderer while creating in xpans.

### Using channel-based synthesizers and/or effects
Channel-based synthesizers and effects pan audio signals across multiple output
channels. By converting those channels into audio sources, you will create
phase interference. Always separate individual voices into their own
audio sources or reach for spatially-aware audio plugins that use the
xpans Spatial Property Exchange (SPE).
