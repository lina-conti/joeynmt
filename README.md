# &nbsp; ![Joey-NMT](joey2-small.png) Joey NMT with option to deactivate teacher

:koala: This repository is forked from [joeynmt/joeynmt](https://github.com/joeynmt/joeynmt). 

As part of my [internship with Neuroviz](https://github.com/lina-conti/neuroviz-internship), I added an option to deactivate teacher forcing — that is, to use the predicted prefix instead of the gold prefix during training.

The only file that was modified with respect to the original version is `joeynmt/models.py`.

## Usage
To find detailed information about the usage of JoeyNMT, see [the original README](https://github.com/joeynmt/joeynmt) and [the official documentation](https://joeynmt.readthedocs.io).

To deactivate teacher forcing during training, in the `model` section of the YAML config, set `teacher_forcing` to `"off"`. By default, `teacher_forcing` is set to `"on"`.
