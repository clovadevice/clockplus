# Clock+ Opensource 

# How to build

1. Get apps_proc from codeaurora
   ```
   repo init -u https://source.codeaurora.org/quic/le/le/manifest.git -b release -m LE.UM.3.3.1.r1-06800-qcs405.0.xml --repo-url=git://codeaurora.org/tools/repo.git --repo-branch=caf-stable
   ```

2. Download the kernel
   ```
   git clone https://github.com/clovadevice/clockplus.git
   ```

3. Build
   ```
   cd kernel/msm-4.14
   make mrproper
   make ARCH=arm vendor/qcs405_defconfig
   make menuconfig
   make all
   ```

# License
Please see [licenses](licenses) and [licenses/License_CLOVA.txt](licenses/License_CLOVA.txt) for the full list of the open source software modules and licenses. 


