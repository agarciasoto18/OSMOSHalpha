# OSMOSHalpha

1. This code takes the spectroscopic data from OSMOS
2. The FITS files are read with readmultispec.py from https://github.com/kgullikson88/General/blob/master/readmultispec.py
3. The radial velocity is found by fitting the Halpha line with a guassian. This uses specutils and astropy but the goals it replace this part with scipy's curve_fit
4. The spectra is shifted to account for movement and systematics.
4. The Error calculation code is underconstruction but was created with the guidance of code from https://github.com/tboudreaux
6. The Halpha Equivalent widths are found with eqwidth.py within Professor Elisabeth Newton's ernlib library: https://github.com/ernewton/ernlib/blob/master/eqwidth.py
