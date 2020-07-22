Thanks to all the developers that have made this happen.

My system:

        Asrock x570 Creator
        Ryzen 9 3900
        Radeon Pro W5700
        2 x 32gb DDR4-3200 ECC
        2 x NVME drives

Kexts:

        AMDRyzenCPUPowerManagement.kext
        AppleALC.kext
        AppleMCEReporterDisabler.kext
        HibernationFixup.kext
        Lilu.kext
        MacProMemoryNotificationDisabler.kext
        NVMeFix.kext
        RadeonBoost.kext
        RealtekRTL8111.kext
        SMCAMDProcessor.kext
        SmallTreeIntel82576.kext
        USBPorts-X570-ASRock-CR-Int_BT.kext
        USBPorts-X570-ASRock-CR-PCIe_BT.kext
        VirtualSMC.kext
        WhateverGreen.kext
        itlwmx.kext

What works:

        Audio
        Wifi
        GFX
        Storage
        USB
        10gbe and 1gbe

What doesn't work:

        Sleep
        Thunderbolt 3

What hasn't been tested:

        Bluetooth

Notes:

        I had to use iMacPro1,1, MacPro7,1 does not work
        I had to add agdpmod=pikera to bootargs for my GFX card (Navi 10)
        I successfully chainloaded the opencore efi to my grub so now I can triple boot windows, linux, mac
        I basically took iGPU's github and updated it and included my own DSDT.aml and serials
        I created an offline installer from a virtual machine to install it
        I haven't tested without RadeonBoost, but performance seems to be on par with Windows in WoW
        I installed directly from 10.15.6, it wasn't an upgrade
