# for python packages installation #

- python 3.11 only supports torch 2.x version whereas source v5.0.3 only available in older torch version(less 1.13.1)
  - use python 3.7(.16)
  - pip install torch==1.13.1+cu116 torchvision==0.14.1+cu116 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu116

- source v5.1.1 use torch 2.1.0
  - use python 3.11(.13)
  - pip install torch==2.1.0 torchvision==0.16.0 torchaudio==2.1.0 --index-url https://download.pytorch.org/whl/cu121

- for Windows support nvidia gpu, recommanded using anaconda to install tensor accelerations.
  - python inference.py --gpu 0 --input xxx.wav

- for Mac M1, librosa will compile during the installation, 
  - ensures openblas installed via homebrew
  - check and export the pkg config path from /opt/homebrew/opt/openblas/lib/pkgconfig for menson build
  - NOTE: OpenBLAS has been partial of Xcode SDK Accelerate componment


