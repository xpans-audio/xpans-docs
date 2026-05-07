# Rendering

Rendering can be thought of as having two stages: Source Interpretation and
Sample Processing.

Source Interpretation is when an audio source's spatial data is transformed
into values that the Sample Processing stage will use to modify and output
audio samples. The result of Interpretation is also called an interpretation.
Interpretations vary in the type of data they hold as they are specifically
for the target rendering format.

Interpretation does not interact with audio data, and Sample Processing does
not directly interact with spatial data. Interpretations are intermediate
data that sit between Interpretation and Sample Processing.

This separation of stages allows Interpretation to happen only when necessary.
If an audio source's properties are unchanged, it does not need to be
re-interpreted (except in cases where the scene transforms relative to the
listener, i.e. headtracking).
