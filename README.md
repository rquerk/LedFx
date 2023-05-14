# LedFx
LedFx install script for Arch Linux

Tested on Manjaro Xfce Minimal Installation
original script: https://install.ledfx.app

My changes:
  using pacman instead of apt
  renaming deb packages to their pacman equivalent
  
  installing aubio via pacman and pip
    reason: installing aubio as dependency fails with error in pip "Failed building wheel for aubio" or error in gcc "'avFormatCtx' will never be NULL"
  
  installing pkgconfig package
    reason: missing pkg-config when trying to execute pip install ledfx
  
  not installing libatlas3-base, libavformat58
    reason: no such packages available; you might need ffmpeg?
  
