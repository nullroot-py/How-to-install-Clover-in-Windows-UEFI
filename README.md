# How-to-install-Clover.
How To Install Clover tutorial in Windows(UEFI Only):
<br/>
<br/>
<br/>
Step 1: 
<br/>
Download Clover Bootloader ISO file from here: https://sourceforge.net/projects/cloverefiboot/files/Bootable_ISO/
<br/> 
The file will be in a compressed format called lzma, with a .lzma extension. 
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
Step 4:
Open Notepad ***in Administrator***.
<br/>
Do the open or open with command and go to SYSTEM partition and open it. In the partition there is a Folder called EFI and open it. Create a folder called 'Clover' or you may call it whatever you want, but I just 'Clover' for simplicity's sake. Copy those EFI, Library and usr folders from Step 2 and paste them in the Clover folder. After you copied the files into Clover, X out of the Open and exit out of Notepad or the program you are using. We're still not done yet.
<br/>
<br/>
<br/>
Step 5: Install Hasleo EasUEFI, I used Trial version. Click 'Manage EFI System partition'
