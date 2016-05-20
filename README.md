# STB8000_TDT_SH4
This is version Duckbox TDT SH4 for Albis STB8000(ufs913).

How To..
1. Clone git repo
    git clone https://github.com/Raxone/STB8000_TDT_SH4.git

2. cd STB8000_TDT_SH4

3. Install dependency
    sudo ./prepare4cdk.sh 

4. cd STB8000_TDT_SH4/cdk

5. make dir cdk/root/boot and put in boot dir audio.elf and video.elf from stb and rename it in audio_7105.elf and video_7105.elf

6. Configure and build
    ./make.sh

