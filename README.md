# auto h-encore
A C# (.NET) application to automate (most of) the process of getting h-encore running on your PS Vita system!

This application is **WINDOWS ONLY**.

![screenshot](https://puu.sh/AQ17U/b204b8f5fa.png "screenshot")

## Features
This application does everything short of installing QCMA/integrating libVitaMTP. That means:

 - Automatically downloads required tools (psvimgtools, pkg2zip, bittersmile demo and h-encore itself)
 - Allows user to import necessary files if they've already downloaded them *(optional)*
 - Grabs CMA encryption key from your account ID
 - Unpackages bittersmile and repackages it with your encryption key and h-encore
 - Trims excess bittersmile demo files to reduce h-encore filesize from ~240MB to ~17MB *(optional)*
 - Moves finished files to your QCMA directory for copying to your PS Vita
 
This application **does not**:
 
 - Get your AID automatically
 - Send h-encore to your PS Vita
 
Basically, you still need QCMA.

## Usage

The application has been verified working on 1000 and 2000 series Vita's as well as PSTV.

Requires .NET 4.5.2 or higher (Windows should automatically download it or link you to it if you don't have it)

Download and extract the [latest release](https://github.com/noahc3/auto-h-encore/releases "latest release") and run it. Further instructions are included in the application itself. QCMA is required to get your AID and transfer h-encore to your Vita.

If the application crashes or h-encore fails to install, please [submit an issue](http://https://github.com/noahc3/auto-h-encore/issues "submit an issue"), **do not create an issue on the h-encore Github**, it probably isn't their fault.

## Build

Clone the repository and open the solution in Visual Studio. Build from there.

## Contributing

I don't know C, so I can't reasonably integrate libVitaMTP into the application to fully automate the process. If you can do this, I would greatly appreciate it if you could fork and/or submit a pull request to implement this functionality. 

The code also needs some cleanup and better error handling.

Other changes are also welcome through pull requests.

## Thanks
 - thefl0w for [h-encore](https://github.com/TheOfficialFloW/h-encore "h-encore") and all of their other contributions to the Vita scene.
 - yifanlu for [psvimgtools](https://github.com/yifanlu/psvimgtools/) and all of their other contributions to the Vita scene.
 - mmozeiko for [pkg2zip](https://github.com/mmozeiko/pkg2zip "pkg2zip").
 - Everyone else that positively contributes to the Vita scene.