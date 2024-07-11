## Window Hypervisor Platform

Windows Hypervisor Platform (WHP) is required to run the Windows x86 emulator.

### PowerShell

Open PowerShell with administrator privileges and run:
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName HypervisorPlatform
shutdown -r -t 0 #if it didn't reboot
```

### Optional Features

Open `optionalfeatures` and tick `Windows Hypervisor Platform` and press OK. Restart when asked.

![image](https://github.com/zalnaRs/LibHMOS-NEXT/assets/53659756/8ee496e5-ed8d-4bcf-aed9-d4c487a5bbcf)
