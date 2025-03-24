Natural Language to BPMN - Generation of BPMN Processes from Natural Language Descriptions
============================================================================================

This repository provides the training dataset, the natural language descriptions used to
evaluate the approach, and the source code of the implemented prototype of the approach
presented in the paper "Automated Generation of BPMN Processes from Textual Requirements",
submitted to the Transactions on Software Engineering (TSE) journal.

DATASETS directory
============================================================================================
The DATASETS directory contains two sub-directories: the EXPERIMENTS directory and the
TRAINING directory.

* EXPERIMENTS directory: This directory contains all the natural language descriptions used to evaluate the approach.
25% of them come from the PET dataset or other proceedings, while 75% of them were handcrafted by the experts who tested the tool

* TRAINING directory: This directory contains all the training data that was used to fine-tune GPT.
Each file starting with the letter 'q' is a training file, while each file starting with the letter 'v' is a validation file.
The files 'train_file.train' and 'valid_file.valid' are aggregated versions of the other files.
Each file is composed of two parts: a description of the process (or user prompt for GPT) visible above the "ASSISTANT:" tag, and a set of expressions (or assistant prompt for GPT) corresponding to the expected output of GPT for the given description (visible below the "ASSISTANT:" tag). 

TOOL directory
============================================================================================
This directory will contain the source code of the prototype used in this approach.
It is worth noting that one CAN NOT make usage of this source code as it requires the authors' personal OpenAI API key to work.
However, anyone interested can duplicate this source code, fine-tuned his own model and make usage of this source code.

Contributors
============================================================================================

* [Quentin Nivon](https://quentinnivon.github.io/)
* [Gwen Salaün](http://convecs.inria.fr/people/Gwen.Salaun/) 

License
=============================
TODO
