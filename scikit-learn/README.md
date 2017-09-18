# scikit-learn

This creates an image from the latest version of Python and all necessary dependencies for using the scikit-learn machine learning framework including Jupyter Notebook.  The setup corresponds closely to that defined in the **Introduction to Machine Learning with Python** book by A C Muller and S Guido.

It is configured with:

* NumPy
* SciPy
* Pandas
* Matplotlib
* Graphviz
* Pillow
* IPython
* Jupyter
* scikit-learn
* mglearn

To start a container straight into Jupyter Notebook run:

`docker run -it --rm bwhazel/scikit-learn`

To load the notebook copy the URL, including token, from the command-line.

Alternatively, to start a container at a shell prompt run:

`docker run -it --rm bwhazel/scikit-learn bash`

To work with Python files outside of the container attach a volume to the desired location:

`docker run -it --rm -v /path/to/host/directory:/path/in/container bwhazel/scikit-learn bash`

To run Jupyter Notebook from the shell in a container a couple of additional flags are required:

`jupyter notebook --allow-root --ip "*"`