# framer
framer is intended to adjust a sequence of images in order to create a video with a fixed framerate. To do that it interpolates missing frames, removes unnecessary frames and creates a numeric sequence of files. Images must be in the format 'second_frame-in-second.extension' in order to work properly.

Usage: framer -f 20 -e jpeg -r

-h        Show HELP (this output)
-f [NUM]  Sets input framerate. Default is 24.
-e [STR]  Sets extension. Enter the extension without the period. Default is tga.      
-r        Create a final sequence from '1.extension' to 'end.extension'
