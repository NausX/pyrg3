About
=====
This script is colorized to Python's UnitTest Result.
inspired by RedGreen(rg command)

Adapted for `python3` by NausX.


Install
=======
Just add it to your working directory?

I haven't bother making a python package for it so far, you can just clone it
and run `make install`.

pip install git+git://github.com/NausX/pyrg3#egg=pyrg3 seems a solution but I
never used it so far. I'll come back on this later.



Require
=======
* Python3.5 +


Usage
=====
basic usage::

  $ pyrg TEST_SCRIPT.py

  $ python TEST_SCRIPT.py |& pyrg

verbose print usage::

  $ pyrg -v TEST_SCRIPT.py

  $ python TEST_SCRIPT.py -v |& pyrg

specified testcase::

  $ pyrg TEST_SCRIPT.py TestCase.test_foo


Configuration
=============
setting to $HOME/.pyrgrc file.
setting file example::

    [color]
    ok = green
    fail = yellow
    error = red
    function = cyan

you can be used color keywords are::

    black gray red pink darkred green yellowgreen
    darkgreen brown yellow gold blue lightblue
    darkblue magenta lightmagenta darkmagenta
    cyan lightcyan darkcyan silver white darksilver

