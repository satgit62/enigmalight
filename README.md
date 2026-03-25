# EnigmaLight Customized installation package for VU+ 4K with VTI IMAGE. 

An Ambilight clone for broadcom based linux receivers.

* EnigmaLight for 4K receivers with ARM architecture consists of two installation packages: 'EnigmaLight Plugin' and 'EnigmaLight Binary'.

These have now been updated and adapted for VU+ 4K receivers with VTI-Imagine and combined into a single installation package (IPK).

* EnigmaLight for VU+ receivers with MIPS architecture and VTI-Imagine has also been updated and provided with the correct binary file.

When installing, be sure to use the correct IPK installation package (ARM/MIPS), as they are not compatible with each other.

-----------------------------------------------------------------------------------------------------------------------
# How to install

Any previous EnigmaLight installations must be uninstalled first.

Transfer the installation packages appropriate for your box via FTP to  `/tmp/` and  then install via the terminal command line:

```
opkg remove enigma2-plugin-extensions-enigmalight
opkg remove enigmalight
opkg update
opkg install /tmp/*.ipk
```

If everything is correct, you should see output similar to this in the terminal/SSH, see Pcture:

<img width="1095" height="880" alt="EnigmaLight Install" src="https://github.com/user-attachments/assets/4d9ee581-85ed-49fc-b94a-d9803e587aa6" />


# Note
-For some devices like Wled, Hyperk, Atmolight, Karatelight, Adalight you need this kernel modules:
> **ch341**, **cp210x**, **cdc-acm**, **ftdi-sio**

You can access the kernel modules via the Plugin Browser > Manage Extensions > Install/Remove Software Packages > Kernel Modules. 

Reboot your receiver and if all is succesfull you can make a configfile and run it.

Enjoy!
