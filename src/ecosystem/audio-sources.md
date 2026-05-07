# Audio Sources

An audio source is a combination of one audio channel and spatial metadata
that describes the spatial properties of the audio channel. 
In other ecosystems, this concept is known as Object-based audio.

## Properties

### Position
Each audio source has a three-dimensional position within virtual space. This is
typically represented using X, Y, and Z coordinates, although other coordinate
systems can be used.

#### Cartesian orientation
Currently, our official software uses left-handed, z-up coordinates.

### Extent
An audio source may have an extent, which can be thought of as its size.
This determines the space an audio source will occupy in a scene.

> Currently, extent is only scarcely (and in some places, incorrectly) 
> implemented in the ecosystem. More work needs to be done to find suitable
> algorithms for correctly solving extent's effect in each rendering mode,
> especially directional rendering modes like directional stereo and 
> headphones.

### Shape
Each audio source with extent above zero in more than one axis must have an
explicitly and unambiguously defined shape. An audio source with extent but
without shape is invalid within the xpans Ecosystem.

> Currently, only cuboidal shapes are implemented as we have yet to decide how to
> represent and render other shapes.

### Rotation
Audio sources with extent and shape may also have a rotation. This determines
the rotation of a source's extent around with its position as its origin point.

> Currently, rotation is completely unimplemented. This is because it depends
on extent to have any effect, and extent still has many unsolved implementation
challenges.

## Audio sources in motion
Just like audio data, spatial data is sampled at a particular rate. xpans does
not have a concept of a separate spatial sampling rate. Instead, spatial
samples can exist at the same time as any audio sample. This allows for extreme
control and precision in how a mix is rendered. However, it can mean a large
amount of spatial data for scenes with lots of frequently moving audio sources.

> While the xpans ecosystem may not enforce a separate spatial sampling rate,
> certain spatial codecs, formats, or user configurations may enforce a spatial
> rate limit to decrease file size and/or increase performance. In such cases, 
> spatial samples and/or renderer interpretations may be interpolated to 
> prevent unwanted artifacts.
