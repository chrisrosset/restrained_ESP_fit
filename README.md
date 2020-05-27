# resp

This is a fork of the `resp` program commonly used in computational chemistry for fitting partial charges to values of the provided molecular Electrostatic Potential (ESP) field around a molecule.
The method was first described by Bayly et al.¹ using the MK mesh of sampling the ESP field² but the program can generally fit charges to any mesh of points.
The mesh needs to be produced independently; see the [jszopi/repESP](https://github.com/jszopi/repESP) repo for some helpers, including extracting ESP fitting points from the output of the Gaussian program and wrapping the calls to the `resp` program in a Python library.

History prior to version 2.2 was not preserved (or rather, reconstructed, considering lack of a version controlled repo).
This version was downloaded in May 2020 from https://upjv.q4md-forcefieldtools.org/RED/ together with other programs in q4md-fft tools 2.0.
The original README for this version can be found in the [`README-2.4.txt` file](https://github.com/jszopi/resp/blob/master/README-2.4.txt) --- see for build instructions.

I am hoping to rewrite this program in Python in order to encourage users to experiment with their own fitting methods.
The code will thus soon be available in PyPI, possibly under a less generic name.
Please open a PR if you'd like it to be available in your system's package manager.

--- 

¹ C. I. Bayly, P. Cieplak, W. D. Cornell and P. A. Kollman, *J. Phys. Chem.*, 1993, **97**, 10269–10280

² U. C. Singh and P. A. Kollman, *J. Comput. Chem.*, 1984, **5**, 129–145