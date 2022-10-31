# The Notemakers

## Project Statement
Musical improvisation in Indian Classical songs varies from more explored techniques such as in Jazz or Blues due to additional restriction or nuance present from musical modes and the instruments being chosen. Our goal would be to design a model that can interpret an audio sample and implicitly recognize the constraints of musical mode and style to generate an improvisational segment of a given input size.

## Methods
### LSTM for generating music

We plan using a series of LSTM's that act as single-step predictors. The network is trained to use hidden layer activations as its memory and, once the problem of vanishing gradients is mitigated, we may seed the model with initial musical input values and have it generare novel improvisations using its outputs to generate subsequent inputs.

### CNN for gauging accuracy
Using the same dataset that the RNN was trained on, we will develop a simple classifier to compare the improvised segment to its input and assess not only its similarity but its validity. Validity will be defined on how accurately it conforms to the implicit musical constraints of the source segment. 

## Innovation
Our project builds on existing research into music generation by extending it to a previously unexplored genre: Indian classical. The presence of new structures, rules, and styles make the generation of Indian classical music a complex task – one which we hope to tackle.
