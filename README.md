# Bypass-

Hi, I currently am working on diffrent projects over diffrent period this one i have to showcase allowed me to stay hidden with my "Insane Skill"
when it comes to Minecraft, Fivem, And different games that will look through your pc to see your "Insane Skill"

Keep in mind some of the program you use to aquire this insane skill will leave behind ceratin words to find it directly
Use this if you have no other way/if the program dosent provide a self-destruct button/gui

Discord; kimikuko

Lmk if you need custom work for those certain programs!

-----------------------------------------------------------------------------------------

Step 1

Download your file that you plan on hidiing and give it a legit name & put it in it's respectful folder!


Go to your downloads or desktop folders, Press new and Press on "Shortcut" 
Paste in the following path:
C:\windows\system32\cmd.exe


Go to absolutely any folder on your computer (Preferably System folders, for example:
C:\Windows
C:\Windows\System32

Move the Shortcut file into one of those folders & Keep the file path to the shortcut. 

Open task scheduler and Extend the "Task scheduler library" using the arrow.

![image](https://github.com/user-attachments/assets/bb5c4f73-476f-4e17-b4c7-1a1353d0bd32)

Extend any folder; next you will find a folder with a alot of little subfolders
Choose on of them a create a task
Rename The task you just made to one of these specially made ones

Schedule Maintenance Work
Schedule Wake To Work
Schedule Work
SvcRestartTask
RefreshCache
PLUGScheduler                     save it ofc.




Press Change users of group; Type in administraotrs and press "check names", if you dont get an error ur good, if u do get one exit out of the change users of group 
Run with highest privilages, Hidden, Configure for: Change it to Windows 10 (Or 11 if you're on 11) 

Set the triggers on User Logon & in Actions paste the path to the shortcut you saved earlier. 
Click and go to Conditions and Turn off "Start only if the pc is on AC power", Turn on "Wake the Computer to run this task" 

Press on OK, Double click on the task again, and save the "Location"





![picture](https://github.com/user-attachments/assets/af53cf93-b918-420e-abb7-a0f6b7c475bf)

----------------------------

Next Find out Bam Directory 

Open registry editor and paste this path at the top:
Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\bam\State\UserSettings
Extend the UserSettings folder using the arrow, Now look through all the subfolders for a folder with alot of registry keys in it.

![Screenshot 2025-03-05 225906](https://github.com/user-attachments/assets/74b7e788-71c1-4fed-9b60-a85b5954355f)

Once you find that folder, Copy the folder path from the top and keep it in a notepad. 

Now right click on the folder you've found, Press Permissions, Go to the "Administrators" Profile (Should be the 2nd one) and Allow Full control

----------------------------

Finally 

Let's first identify the name of the key that would be generated.

Take the path to your "Special File", Remove C: at the start and replace it with: 
\Device\HarddiskVolume3\

So if my Special File is in the path:
C:\windows\system32\Github.exe
It would look like:
\Device\HarddiskVolume3\windows\System32\Github.exe

This is how the command would look like:
reg delete "Path to BAM directory without Computer\ at the start." /v "The key that we identified" /f 
For example: 
reg delete "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\bam\State\UserSettings\S-1-5-21-4160387986-5127848212-1968453011-1001" /v "\Device\HarddiskVolume3\Windows\System32\Github.exe" /f

And now find out Store deletion command:
reg delete "Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\Compatibility Assistant\Store" /v "C:\Path\To\Your\Github.exe" /f 
For example: 
reg delete "Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\Compatibility Assistant\Store" /v "C:\windows\system32\Github.exe" /f



[Alternate Stream View](https://www.majorgeeks.com/files/details/alternatestreamview.html) - Download the file, Scan your Special File path & if there's a ZONE.IDENTIFIER file with your File name in it - click on it and Press on the X at the top. Delete the file. 

Open CMD administrator and run the following command:
Fsutil usn deletejournal /d C: 


------------------------------------------------------

Your Done!

Open CMD as Administrator as soon as your PC starts up. 
and run this command: 
schtasks /run /tn Location\TaskName

Replace Location with the location you saved from the task, Replace TaskName with the Name of the task you chose from the options before. 
A new CMD window should appear.

Close the Old CMD window and type this in the new CMD window.
schtasks /delete /tn "Location\TaskName" /f
Replace Location with the location you saved from the task, Replace TaskName with the Name of the task you chose from the options before. 

Now type in: 
start C:\Path\To\Github.exe
And now run all your reg delete commands.

-----------------------------------

After all said and done when you are in a intense moment where you have to close out all the file Make sure everything suspicious is closed. (Cmd etc)


If your file has a close option use it!!!!





