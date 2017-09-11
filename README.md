# readHyperSpyH5
MATLAB function to import an HDF5 file saved by [HyperSpy](https://github.com/hyperspy/hyperspy)

This MATLAB function is designed to import HyperSpy's saved HDF5 files (`.hspy` extension). 
It is used to easily transfer data from HyperSpy to MATLAB
without losing the axial calibration information.
The underlying data is returned as the primary output, and axis metadata 
(such as names, units, scales, etc.) are returned as supplemental output.

To use the function, place it somewhere on your MATLAB path, and call it
passing a string with the HyperSpy output file name as the only input:
```MATLAB
data = readHyperSpyH5('example_file.hspy');
```

The additional outputs of the script are described in the documentation string for the function.

The script has been tested on 2D and 3D hyperspectral data (spectrum images),
but should work for arbitrarily sized data. Please raise an issue on the
[issue tracker](https://github.com/jat255/readHyperSpyH5/issues) or in the 
HyperSpy [Gitter chat](https://gitter.im/hyperspy/hyperspy) with any problems.

`readHyperSpyH5` was written by [Joshua Taillon](https://www.nist.gov/people/joshua-taillon)

[Download readHyperSpyH5](https://raw.githubusercontent.com/jat255/readHyperSpyH5/master/readHyperSpyH5.m)
