# hNews_k

#### Table of Contents

* 1
* 2
* 3
* 4

## Presentation

This work tries to reproduce the results of [A Neural Conversational Model](http://arxiv.org/abs/1506.05869) (aka the Google chatbot). It uses a RNN (seq2seq model) for sentence predictions. It is done using python and TensorFlow.

## Installation

The program requires the following dependencies (easy to install using pip):
 * python 3.5
 * tensorflow (tested with v0.9.0)
 * numpy
 * CUDA (for using gpu, see TensorFlow [installation page](https://www.tensorflow.org/versions/master/get_started/os_setup.html#optional-install-cuda-gpus-on-linux) for more details)
 * nltk (natural language toolkit for tokenized the sentences)
 * tqdm (for the nice progression bars)
 
## Running

The loading corpus part of the program is inspired by the Torch [neuralconvo](https://github.com/macournoyer/neuralconvo) from [macournoyer](https://github.com/macournoyer)

### MediaWiki

To train the model, simply run `main.py`. Once trained, you can test the results with `main.py --test` (results generated in 'save/model/samples_predictions.txt') or `main.py --test interactive` (more fun).

## License

Creative Commons Public Domain License, the original at http://creativecommons.org/licenses/publicdomain/ or any later version published by Creative Commons; with either a waiver of rights, or an assertion that no rights attach to a particular work.
# hNews_k
