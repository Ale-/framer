# framer
framer is intended to adjust a sequence of images in order to create a video with a fixed framerate. To do that it interpolates missing frames, removes unnecessary frames and creates a numeric sequence of files. Images must be in the format 'second_frame-in-second.extension' in order to work properly. For example `1_15.tga` would be the 15th frame in the first second. 

## Usage
Use it doing, for example:
```bash
framer -f 20 -e jpeg -r
```
This way you'd create a lineal numbered sequence from 1.jpg to (end).jpg intended to create a video with a fixed framerate of 20 fps.

### Parameters
* `-h`        
Show help
* `-f [NUM]`  
Sets input framerate. Default is 24.
* `-e [STR]`  
Sets extension. Enter the extension without the period. Default is tga.      
*  `-r`        
Create a numbered lineal sequence from '1.extension' to 'end.extension'

## Install
To use it download it, and make it executable with:
```bash
sudo chmod+x framer
```
You could move it to a bin folder (or another folder in the PATH of the system), for example bin in your user folder:
```bash
mv framer ~/bin
```
