# LedFx
LedFx install script for Arch Linux

Tested on Manjaro Xfce Minimal Installation<br>
original script: https://install.ledfx.app

My changes:<br>
  using pacman instead of apt<br>
  renaming deb packages to their pacman equivalent
  
  installing aubio via pacman and pip<br>
    reason: installing aubio as dependency fails with error in pip "Failed building wheel for aubio" or error in gcc "'avFormatCtx' will never be NULL"
  
  installing pkgconfig package<br>
    reason: missing pkg-config when trying to execute pip install ledfx<br>
  
  not installing libatlas3-base, libavformat58<br>
    reason: no such packages available; you might need ffmpeg?
  
