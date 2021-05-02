# How-to-install-Clover-in-Windows-UEFI
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
Step 5: Install Hasleo EasUEFI, I used Trial version. Click 'Manage EFI Boot Option'
<br/>
Left of Detailed information, there are a bunch of buttons. Click the second, which looks like a table/calendar and a green plus on it. It will create a boot entry. Make it type 'Linux or Other OS' and name it Clover. Click the grey circle to choose where our efi file is. I have a Windows laptop with an external HDD that contains my Linux, so i have 2 EFI partitions, each on a drive. Click the one that has the Clover boot loader files, which is probably the first one. Click Bowse on the bottom part of the Window and click the plus to open folders. Go to EFI, Clover, EFI, Boot and select Bootx64.efi. Then click Ok. It will be at last of the list, so click the up arrow to move it up at the top. Done!
