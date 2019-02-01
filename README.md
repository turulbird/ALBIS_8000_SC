# ALBIS_8000_SC
  (STB8000_TDT_SH4 update)
  
This is version Duckbox TDT SH4 for albis SceneGate 8000 (ufs913).

This build or (https://github.com/Duckbox-Developers) is not builds for final firmware.

This builds if for easy build and modified driver,kernel or python plugin for enigma and put/change in basic HDMU or another firmware for ufs913 etc.

The version of builds is modified kernel and drivers for albis SC 8000 and need HDMU firmware for ufs913.

In ufs913 HDMU firmware change drivers and kernel to work on albis SC 8000.


How To..

1. Clone git repo

    git clone https://github.com/turulbird/ALBIS_8000_SC.git
    
2. cd ALBIS_8000_SC

3. Install dependency
    
    sudo ./prepare4cdk.sh 

4. cd ALBIS_8000_SC/cdk


5. make dir cdk/root/boot and put in boot dir audio.elf and video.elf from stb and rename it in audio.elf to audio_7100.elf, audio_7105.elf, audio_7109.elf and audio_7111.elf, video.elf to video_7100.elf, video_7105.elf, video_7109.elf and video_7111.elf.

6. Configure and build

    ./make.sh

28

5

y

2

4

1

1

make crosstool driver -jx

(To build kernel,toolchain and driver configured for albis SC 8000)

or

make yaud-enigma2-pli-nightly -jx

(-jx = use x cpu core if got more set it -j8)
(this build all)


Choose between the following revisions:
========================================================================================================
 0) Newest                 - E2 OpenPli gstreamer / libplayer3    (Can fail due to outdated patch)     
========================================================================================================
 1) Use your own e2 git dir without patchfile
========================================================================================================
 2) Mon, 17 Aug 2015 07:08 - E2 OpenPli gstreamer / libplayer3 cd5505a4b8aba823334032bb6fd7901557575455
========================================================================================================
Media Framework : gstreamer
External LCD    : no
Select          : 2

On error try rerun.
