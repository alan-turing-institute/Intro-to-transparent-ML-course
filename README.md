# An Introduction to Transparent Machine Learning

[![Build Stats](https://github.com/pykale/transparentML/workflows/deploy/badge.svg)](https://github.com/pykale/transparentML/actions)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](https://github.com/pykale/transparentML/graphs/contributors)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

This repository contains a Jupyter book on [An Introduction to Transparent Machine Learning](https://www.turing.ac.uk/introduction-transparent-machine-learning), part of the [Alan Turing Institute](https://www.turing.ac.uk/)'s [online learning courses in responsible AI](https://www.turing.ac.uk/funding-call-online-learning-courses-responsible-ai). It is developed as [a PyKale repository](https://github.com/pykale/transparentML) for deployment as [an Alan Turing Institute repository](https://github.com/alan-turing-institute/Intro-to-transparent-ML-course/).

The latest development version of this book is available at [pykale.github.io](https://pykale.github.io/transparentML/) and the latest stable version is deployed at [alan-turing-institute.github.io](https://alan-turing-institute.github.io/Intro-to-transparent-ML-course).

Welcome your feedback and contribution via opening [issues](https://github.com/pykale/transparentML/issues), [discussions](https://github.com/pykale/transparentML/discussions), and/or [pull requests](https://github.com/pykale/transparentML/pulls).

&copy; Haiping Lu and Shuo Zhou

## Building the book locally

If you'd like to develop and/or build this book locally, you should:

1. Clone the [source repository at PyKale](https://github.com/pykale/transparentML): `git clone https://github.com/pykale/transparentML`.
2. Run `pip install -r requirements.txt` to install the required dependencies for building the book (it is recommended you do this within a virtual environment).
3. (Optional) Edit the book source files located in the `content` directory.
4. Run `jupyter-book build content` from the project directory `transparentML` to build the book.

A fully-rendered HTML version of the book will be built in `content/_build/html/`.

## Contributing

This repository uses [`pre-commit`](https://pre-commit.com/). If you will contribute to this repository (most welcome!), please install `pre-commit` and run `pre-commit install` prior to committing. If you have already committed, but your PR is failing because of a pre-commit error, run `pre-commit run --all` locally to inspect and fix the error.

## Contributors

We welcome and recognise all contributions. Please see our [Contributor Guidelines](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md) for more information. You can see a list of current contributors in the [contributors tab](https://github.com/pykale/transparentML/graphs/contributors).

## Credits

This project is created using the excellent open source [Jupyter Book project](https://jupyterbook.org/) and the [executablebooks/cookiecutter-jupyter-book template](https://github.com/executablebooks/cookiecutter-jupyter-book).

## License

All content except for YouTube videos is released under the [MIT License](https://github.com/pykale/transparentML/blob/main/LICENSE). YouTube videos are embedded according to [YouTube's Terms of Service](https://www.youtube.com/static?gl=CA&template=terms).
