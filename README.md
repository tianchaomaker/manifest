DaytonaHTCMania CyanogenMod Build
==================================

1) You need:
------------

- 100GB on HDD
- Linux 64 bits
- Internet connection
- Time
- Patience

2) Installation of the required packages:
-----------------------------------------


  sudo apt-get install git-core gnupg flex bison gperf build-essential \
  zip curl libc6-dev libncurses5-dev:i386 x11proto-core-dev \
  libx11-dev:i386 libreadline6-dev:i386 libgl1-mesa-glx:i386 \
  libgl1-mesa-dev g++-multilib mingw32 openjdk-6-jdk tofrodos \
  python-markdown libxml2-utils schedtool pngcrush xsltproc zlib1g-dev:i386
  
And:

  sudo ln -s /usr/lib/i386-linux-gnu/mesa/libGL.so.1 /usr/lib/i386-linux-gnu/libGL.so
  

3) Create folder and download the source code:
----------------------------

Creating the folder:

mkdir Source

Go to folder:

cd Source

Initialize your local repository using these sources, use a command like this:

    repo init -u git://github.com/DaytonaHTCMania/manifest.git -b kitkat

Then download source:

    repo sync

4) Build the source code:
-------------------------

Go to your source -> cd Source (on Terminal)

Push this command: . build/envsetup.sh

This: lunch

And this: brunch DEVICE (your device replaces "DEVICE")

And wait... if compilation is complete, the ROM is on out/target/product/DEVICE
