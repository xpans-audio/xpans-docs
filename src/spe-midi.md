# SPE-MIDI

SPE-MIDI implements the SPE protocol using MIDI System Exclusive messages for
use in hosts and plugins that don't natively support SPE. It is currently the
only way to use SPE.

SPE-MIDI messages must be manually routed by the user. While audio data
requires each audio source to have its own dedicated audio channel,
SPE does not require a separate MIDI channel for each audio source.
Each SPE-MIDI message includes the audio channel number it refers to.
This number is referred to the 'Source ID'. SPE-MIDI-enabled plugins will
likely require you to provide source IDs.

Unfortunately, without native SPE integration or generic inter-plugin/host
communication, we must tediously ensure our source IDs align with our
audio channels using SPE-MIDI.

Refer to SPE-MIDI's 
[source code repository](https://github.com/xpans-audio/xpans_spe_midi)
for a more technical overview and a rough specification.
