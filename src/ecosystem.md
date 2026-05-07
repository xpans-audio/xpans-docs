# The xpans Ecosystem

xpans is an open ecosystem for source-based spatial audio technologies.
Audio sources have 3D positions in virtual space, and can have several other
spatial properties.

## Philosophy

### Unassuming
xpans aims to make as little assumptions as possible about both creators and 
listeners.

As an ecosystem, xpans does not assume where the listener may be positioned
within a scene. While the ecosystem at its core doesn't make this assumption, 
directional rendering modes (i.e. directional stereo, surround sound) *do* 
render audio sources depending on a central listening position. So keep in mind 
that different rendering modes have their own different constraints as they 
are designed for different listening configurations.

### Objective
xpans' rendering modes are intended to do just enough to create an immersive
experience, remaining simple and predictable.

This principle ensures creators have control over how their mix sounds and can
more easily predict how their mix would sound in a rendering mode they haven't 
monitored. Rendering modes can filter and delay audio signals just enough to 
provide a convincing spatial impression, being sure not to make artistic 
choices on behalf of the creator.

### Open
While describing xpans as an 'open' ecosystem can refer to it being open-source,
it mainly refers to its focus on interoperability, extendability, and 
possibility to be implemented by anyone.

There isn't a strong concept of 'official' technologies within the ecosystem.
If a technology shares the same concept of an audio source (or even a subset) 
and interoperates well with other technologies within the ecosystem, 
then it's probably safe to say it's part of the xpans Ecosystem 
in at least one way or another.
