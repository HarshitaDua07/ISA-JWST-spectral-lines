# ISA-JWST-spectral-lines
JWST MIRI Spectral Analysis Summary of NGC 7469
Prepared by: Harshita Dua
Overview
This project involved analyzing spectral cubes from the JWST MIRI instrument for the Seyfert 1 
galaxy NGC 7469. Using Python tools such as astropy, regions, and matplotlib, we 
extracted and compared spectra from the active galactic nucleus (AGN) and the circumnuclear 
star-forming ring. Through this, we aimed to characterize the mid-infrared emission from these 
physically distinct regions and explore their astrophysical drivers.
Observations
1. Spectral Cube Processing:
o The MIRI data cube was accessed from a FITS file.
o World Coordinate System (WCS) information was used to align sky regions.
o DS9 region files were loaded to define circular areas (using CircleSkyRegion) 
on the galaxy.
o Spectra were extracted by averaging pixel values across each spatial region at 
each wavelength layer in the cube.
2. Spectral Extraction Code Insight:
o A wavelength array was computed from FITS header parameters (CRVAL3, 
CDELT3, CRPIX3) and converted to microns.
o Circular masks were applied to extract 1D spectra from each selected region.
o Plots showed clear variation between the central AGN and star-forming ring.
3. Channel-Specific Resolution:
o Channel 1 (~5.8 pc per pixel): High spatial and spectral resolution, fine structure 
easily resolved.
o Channel 4 (~21 pc per pixel): Resolution drops, with broader features and 
increased noise.
4. Spectral Behavior:
o Central Region: High-ionization lines, steeper continuum, and strong warm dust 
emission.
o Star-forming Ring: Dominated by PAH emission features, indicating UV-excited 
gas.
