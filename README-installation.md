# for python packages installation #

- python 3.11 only supports torch 2.x version whereas source only only available in older torch version(less 1.13.1)

- for Windows support nvidia gpu, recommanded using anaconda to install tensor accelerations.

- for Mac M1, librosa will compile during the installation, 
  - ensures openblas installed via homebrew
  - check and export the pkg config path from /opt/homebrew/opt/openblas/lib/pkgconfig for menson build
  - NOTE: OpenBLAS has been partial of Xcode SDK Accelerate componment


