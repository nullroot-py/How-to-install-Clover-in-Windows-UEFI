# How-to-install-Clover.
How To Install Clover tutorial in Windows:
<br/>
<br/>
<br/>
Step 1: 
<br/>
Download Clover Bootloader ISO file from here: https://sourceforge.net/projects/cloverefiboot/files/Bootable_ISO/
<br/> 
The file will be in a compressed formar called lzma, with a .lzma extension. 
<br/>
Note: The ISO files are from 2019, use Clover Configurator to update Clover accordingly. 
<br/>
<br/>
<br/>
Step 2: Open the lzma, then tar and lastly the ISO file, I used 7-zip to do that. Copy the EFI, Library and usr to a temporary location to copy them to the EFI partition, or do this step in step 4.
<br/>
<br/>
<br/>
Step 3: Execute these commands in Administrator Command Prompt to mount EFI System Partition:
  <br/>
  <br/>
  list disk
  <br/>
  select disk 0
  <br/>
  list partition
  <br/>
  select partition 1
  <br/>
  assign letter=X
  <br/>
  exit
  <br/>
  <br/>
Go to file explorer and make sure that there is a new partition called SYSTEM with assigned letter being X.
<br/>
<br/>
<br/>
