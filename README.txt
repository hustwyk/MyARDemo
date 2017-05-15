MyARDemo 0.0.1

INTRODUCTION
===============================================================================
This is a version of the markerless augmented reality demo modified from NAR. 
The original author is Nghiaho, and thanks for his demo. :)



COMPILING
===============================================================================
To compile you need the following libraries installed

- OpenCV 2.3.x (or above)
- Boost C++ libraries
- Irrlicht Engine

The Linux project can be compiled by opening the NAR_Demo.cbp project in 
CodeBlocks. 

The Visual Studio 2010 project can be found in the VisualStudio2010 directory. 
You will need to modify the paths to the libraries to match your system.

I've only tested the code using a 64 bit compiler. If you have a 32 bit compiler
you need to edit NAR/NAR_Config.h and comment out #define USE_SSE4. I use the
POPCNT assembly instruction, which seems to be only available with 64 bit.


USAGE
===============================================================================
You will need to supply your own AR object image, which must be at the path
    media/AR_object.png
	 
NAR_Demo will not run without this file. It will report an error in the console.
The image should be no larger than the video input size. The easiest way to do
this is to find some software that can access your webcam/camera, hold the 
AR object in front, and take a snapshot. Then crop as required.

You can run NAR_Demo via the console, it does not require any argument. 
On Linux run it via ./NAR_Demo in the root directory and on Windows run 
NAR_Demo.exe. It is recommended you run from a console to get text feedback 
from the program in case of errors.


PRE-COMPILED BINARIES FOR WINDOWS
===============================================================================
For you lucky Windows 64 bit user out there, there is a pre-compiled 
binary NAR_Demo.exe in the root directory. I've included the necessary dlls for 
it to run out of the box.


LICENSE
===============================================================================
Please see the LICENSE file. In summary, it's a BSD license, which means you can
pretty do much whatever you want with the code. For educational or commercial.


FOUND A BUG?
===============================================================================
Email me at hustwyk@gmail.com
