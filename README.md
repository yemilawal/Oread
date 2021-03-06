# Oread
_/ˈɔːrɪad/_

A commandline and GUI tool for the creation of Artemis/Artemis Comparison Tool files.

# Installation
Presently, this package has a number of dependencies:

 - Install a `miniconda` distribution (or anything that allows access to a `pythonw` binary but `miniconda` is recommended (later this tool may be installable via `conda`)

 - Install `biopython` (very easy via `conda` with `$ conda install -c bioconda biopython`)

 - Ensure you have the BLAST+ suite installed (NOT legacy BLAST). Also very easy via `conda`: `$ conda install -c bioconda blast`

 - Finally, the GUI depends on the non-standard module `Gooey`. Install it via `conda` with: `$conda install -c krrishnarraj gooey` or via `pip` with `pythonw -m pip install gooey`


# Running
So far this has only been tested on MacOS. For this, a "framework" version of python is needed.
This can be installed via `conda` which is strongly recommended, and then the script run with the
`pythonw` binary:


    $ pythonw Oread.py

This will open the window. If you set the `Oread.py` script to be executable (it should already be)
and to open with `Terminal` by default (select the file, `Command+I`, then alter the defaults), you can launch
with a double click.

The program can also be run from the commandline by providing the `--ignore-gooey` option to disable the GUI.

    $ python Oread.py --ignore-gooey <...options...>
