This project explores the generation of musical output based on color input.

The algorithm analyzes an RGB color's properties (hue, saturation, value) and
maps these characteristics to corresponding musical elements (key, tempo,
and note velocity). 

This project utilizes a subset of the MAESTRO dataset comprising of 1282 MIDI files. 
All files are parsed with pretty_midi and loaded into an array. 
For each file, the primary melody is extracted, retaining only pitch information (duration and velocity are
omitted).
A k-Markov model was employed to generate melodies that attempt to reflect the ambiance of the input color. 

Dataset: https://storage.googleapis.com/magentadata/datasets/maestro/v2.0.0/maestro-v2.0.0-midi.zip
