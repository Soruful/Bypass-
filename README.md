Contains: 2 bypass methods

1. 1- bypass method 1       ────── ･ ｡ﾟ☆: *.☽ .* :☆ﾟ. ─── = same method ⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི = diffrent steps (still same method)

2. 2- bypass method 2

─── ･ ｡ﾟ☆: *.☽ .* :☆ﾟ. ────── ･ ｡ﾟ☆: *.☽ .* :☆ﾟ. ────── ･ ｡ﾟ☆: *.☽ .* :☆ﾟ. ────── ･ ｡ﾟ☆: *.☽ .* :☆ﾟ. ───

1- 

Download your cheat and give it a legit name & put it in it's respectful folder. 


Go to your downloads or desktop folders, Press new and Press on "Shortcut" 
Paste in the following path:
C:\windows\system32\cmd.exe


Go to absolutely any folder on your computer (Preferably System folders, for example:
C:\Windows
C:\Windows\System32

Move the Shortcut file into one of those folders & Keep the file path to the shortcut. 

Open task scheduler and Extend the "Task scheduler library" using the arrow.





![picture1](https://github.com/user-attachments/assets/1ac1bea1-55f1-473e-b1f7-0dd4a88004b0)



Extend any folder next until you find a folder with alot of little subfolders.
Choose one of them and create a task in them.
Put the name as one of these:
Schedule Maintenance Work
Schedule Wake To Work
Schedule Work
SvcRestartTask
RefreshCache
PLUGScheduler

Save the Task name.
Press Change user or group, Type in Administrators and press "Check Names", if you don't get an error press OK, If u do just exit out of the change user or group. 
Tick Run with highest privilages, Hidden, Configure for: Change it to Windows 10 (Or 11 if you're on 11) 
Make the triggers on User Logon & in Actions paste the path to the shortcut you saved earlier. 
Go to Conditions and Turn off "Start only if the pc is on AC power", Turn on "Wake the Computer to run this task" 

Press on OK, Double click on the task again, and save the "Location"





![picture2](https://github.com/user-attachments/assets/e76796d2-64f2-4c93-bf24-ccc6e22a908c)




⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞  ͜ ◞ ྀི◟⠀ ◞ ྀི◟ ͜ ◞  ྀི◟ ͜  ◞  ͜ ◞ ྀི◟⠀ ◞ ྀི◟ ͜ 
Open registry editor and paste this path at the top:
Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\bam\State\UserSettings
Extend the UserSettings folder using the arrow, Now look through all the subfolders for a folder with alot of registry keys in it.







![picture3](https://github.com/user-attachments/assets/bd126360-0533-43f1-9ff7-151ce8626435)










Once you find that folder, Copy the folder path from the top and keep it in a notepad. 
Now right click on the folder you've found, Press Permissions, Go to the "Administrators" Profile (Should be the 2nd one) and Allow Full control


⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟ 


First of all, BAM command. 
Let's first identify the name of the key that would be generated.

Take the path to your client, Remove C: at the start and replace it with: 
\Device\HarddiskVolume3\
So if my client is in the path:
C:\windows\system32\karma.exe
It would look like:
\Device\HarddiskVolume3\windows\System32\karma.exe
This is how the command would look like:
reg delete "Path to BAM directory without Computer\ at the start." /v "The key that we identified" /f 
For example: 
reg delete "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\bam\State\UserSettings\S-1-5-21-4160387986-5127848212-1968453011-1001" /v "\Device\HarddiskVolume3\Windows\System32\karma.exe" /f

And now let's find out Store deletion command:
reg delete "Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\Compatibility Assistant\Store" /v "C:\Path\To\Your\Cheat.exe" /f 
NT\CurrentVersion\AppCompatFlags\Compatibility Assistant\Store" /v "C:\Path\To\Your\Cheat.exe" /f 
For example: 
reg delete "Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\Compatibility Assistant\Store" /v "C:\windows\system32\karma.exe" /f



Alternate Stream View - Download the file, Scan your cheat's path & if there's a ZONE.IDENTIFIER file with your cheat's name in it - click on it and Press on the X at the top. Delete the file. 
Open CMD as administrator and run the following command:
Fsutil usn deletejournal /d C:
⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟
Restart your PC
Open CMD as Administrator as soon as your PC starts up. 
and run this command: 
schtasks /run /tn Location\TaskName
Replace Location with the location you saved from the task, Replace TaskName with the Name of the task you chose from the options before. 
A new CMD window should appear.
Close the Old CMD window and type this in the new CMD window.
schtasks /delete /tn "Location\TaskName" /f
Replace Location with the location you saved from the task, Replace TaskName with the Name of the task you chose from the options before. 
Now type in: 
start C:\Path\To\Cheat.exe
And now run all your reg delete commands.




⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟⠀ ◞  ྀི◟ ͜  ◞ ྀི◟  ͜  ◞ ྀི◟
Make sure everything suspicious is closed. (Cmd etc)
Destruct your client.

If you're bypassing good screensharers
Open CMD as administrator and run this command:
sc config diagtrack start=disabled
