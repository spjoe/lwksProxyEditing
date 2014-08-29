lwksProxyEditing
================
tool for converting video files for lightworks that can be used for editing and a swaping tool to change video to high quality when finaly rendering the edited movie

This tool converts videos with ffmpeg to the same format as the eyeframe tool.

Usage
===============

The tool consists of three commands:

`lwksProxyClipConverter  files|directories`

if you give as argument one ore more directories the tool check alle files in the directory and if a file has a mimetype with video/* than it gets converted.

`lwksChangeToProxy  directory`


changes all video symlinks in the given directory to Proxy video file. 

`lwksChangeToHigh  directory`

changes all video symlinks in the given directory to High quality video. 
