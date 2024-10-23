# Readme
This repository contains Modus toolbox manifests for RT-Labs components.

## Installation 
Until RT-Labs manifest is added to the official manifest used by Modus Toolbox  
the manifests can be manually added by modifying the ```manifest.loc``` file used by  
the Modus Toolbox installation.

In a typical Modus Toolbox installation on Windows, the ```manifest.loc``` file is  
located on the following path:
```
C:\Users\<user>\.modustoolbox\manifest.loc
```

If not, locate the ```manifest.loc``` file in your installation.

To add RT-Labs components to Modus Toolbox, the path to the super manifest  
part of this repository should be added to the ```manifest.loc``` file. Note that  
the manifest.loc is empty in a typical Modus Toolbox installation.

1. Clone this repo:
```
git clone https://github.com/rtlabs-com/mtb-rtlabs-manifest.git
```

2. Locate manifest.loc and add the path to the RT-Labs super manifest in  
   this repo by adding the line below to ```manifest.loc```:  
   ```C:\Users\<user>\mtb-rtlabs-manifest\mtb-super-manifest-fv2-rtlabs.xml```  

   _Note: This path depends on the user and where this repo was cloned in step 1._

3. Restart ModusToolbox
4. RT-Labs user examples shall now be available in the Modus Toolbox Project Creator.  
   Verify by starting Project Creator and select:  
    - BSP - KIT_XMC72_EVK  
    - Application - Getting Started / Industrial Ethernet 
