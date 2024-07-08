# NOTE: AT THE MOMENT YOU CAN ONLY RUN HARMONYOS NEXT ARM64 ON QEMU
Requirements:
- a Linux distro (We tested it on Ubuntu 22.04)
- a ARM64 CPU
- 8GB+ of RAM

As for now, we have a ARM64 version of HarmonyOS NEXT, here's some specifications:
- There's only the Chinese language
- It can run only on QEMU

# How to test it:

1) Start your Linux (ARM64) Machine

3) Install all the needed packages:
   ```
    sudo apt update && sudo apt upgrade
    sudo apt-get install qemu-system
   ```

4) Download the [Emulation package](https://devuploads.com/vddyjezw9v4j) (**NOTE:** the archive password is "pwp114514")

5) Unzip the Emulation package

6) Run QEMU
   ```
    qemu-system-aarch64 -enable-kvm -machine virt -cpu host -display none -serial stdio -kernel Image -append console=ttyAMA0
   ```
   **Note:**
     - Remove "-enable-kvm" if it gives you an error
     
     - Remove "-cpu host" if your running this into a VM
     
     - Remove "-display none" if you want to see a display output
 
7) Enjoy!

[Home](https://ryzenstechdev.github.io/LibHMOS-NEXT/)
