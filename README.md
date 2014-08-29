# lwksProxyEditing

A tool for converting video files for lightworks that can be used for editing and a swaping tool to change to high quality when finaly rendering the edited movie.

This tool converts videos with ffmpeg to the same format as the eyeframe tool. (eyeframeconverter.wordpress.com)

## Usage

The tool consists of three commands:

`lwksProxyClipConverter  files|directories`

If you give as argument one ore more directories the tool check all files in the directory and if a file has a mimetype with video/* than it gets converted.

`lwksChangeToProxy  directory`

Changes all video symlinks in the given directory to Proxy video file. 

`lwksChangeToHigh  directory`

Changes all video symlinks in the given directory to High quality video. 


## Build and install
  
    mkdir build
    cd build
    cmake -DCMAKE_INSTALL_PREFIX:PATH=/usr ..
    make
    make install
