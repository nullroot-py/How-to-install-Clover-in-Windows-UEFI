# How-to-install-Clover.
How To Install Clover tutorial in Windows:
<br/>
Step 1: 
<br/>
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
<br/>
Download Clover Bootloader ISO file from here: https://sourceforge.net/projects/cloverefiboot/files/Bootable_ISO/
<br/> 
The file will be in a compressed formar called lzma, with a .lzma extension. 
<br/>
Note: The ISO files are from 2019, use Clover Configurator to update Clover accordingly. 
<br/>
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
<br/> 
Step 2: Open the lzma, then tar and lastly the ISO file, I used 7-zip to do that. Copy the EFI, Library and usr to a temporary location to copy them to the EFI partition, or do this step in step 4.
<br/>
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
<br/>
Step 3: Execute these commands in Administrator Command Prompt to mount EFI System Partition:
  list disk
  select disk 0
  list partition
  select partition 1
  assign letter=I
  exit
  
