# LedFx
LedFx install script for Arch Linux

Tested on Manjaro Xfce Minimal Installation<br>
original script: https://install.ledfx.app

My changes:
<ol>
  using pacman instead of apt<br>
  renaming deb packages to their pacman equivalent<br>
  <br>
  installing aubio via pacman and pip
  <ol>
    reason: installing aubio as dependency fails with error in pip "Failed building wheel for aubio" or error in gcc "'avFormatCtx' will never be NULL"
  </ol>
  
  installing pkgconfig package
  <ol>
    reason: missing pkg-config when trying to execute pip install ledfx
  </ol>
  
  not installing libatlas3-base, libavformat58<br>
  <ol>
    reason: no such packages available; you might need ffmpeg?
  </ol>
</ol>
