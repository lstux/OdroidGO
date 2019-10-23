# ino2fw

Create a firmware file (.fw) from an arduino sketch.

It requires :
* Arduino IDE available from [Arduino website](https://www.arduino.cc/en/Main/Software)
* mkfw from [OtherCrashOverride GitHub](https://github.com/OtherCrashOverride/odroid-go-firmware/tree/master/tools), you may use mkfw-build.sh script from this repo to install it
* ffmpeg if you want to use your own application tile instead of default Arduino logo


## Usage
```
ino2fw.sh [options] {sketch_dir|sketch_file.ino}
  Create a .fw file for Odroid-Go from arduino sketch
options:
  -b build_path  : build in build_path [/tmp/ino2fw]
  -t tile.png    : use specified image as tile (resized to 86x48px)
  -l label       : set application label
  -d description : set application description
  -v             : increase verbosity level
  -h             : display help message
 ```
