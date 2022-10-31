# The Notemakers

## Project Statement
Musical improvisation in Indian Classical songs varies from more explored techniques such as in Jazz or Blues due to additional restriction or nuance present from musical modes and the instruments being chosen. Our goal would be to design a model that can interpret an audio sample and implicitly recognize the constraints of musical mode and style to generate an improvisational segment of a given input size. We will then transform this to an Indian classical instrumental audio file.

## Methods
### LSTM for generating music

We plan using a series of LSTM's that act as single-step predictors. The network is trained to use hidden layer activations as its memory and, once the problem of vanishing gradients is mitigated, we may seed the model with initial musical input values and have it generare novel improvisations using its outputs to generate subsequent inputs.

### CNN for gauging accuracy
We will then use a CNN to take the LSTM output and transform it to the style of an Indian flute. This will allow the piano roll and notes generated from the LSTM to be heard in a format where the nuances of the generated music can be shown in full. The CNN will operate on audio spectrograms. 

## Innovation
Our project builds on existing research into music generation by extending it to a previously unexplored genre: Indian classical. The presence of new structures, rules, and styles make the generation of Indian classical music a complex task – one which we hope to tackle.
