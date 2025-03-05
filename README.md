# Bat2Exe-Converter
Simple .bat to .exe converter in Python

:INSTRUCTIONS:

In order to use the 'Bat2Exe Context.py' and 'Bat2Exe.exe' files, a new context action must be created in the .bat right click context menu. This is done by editing keys in the Registry Editor app.

Navigate to the directory 'Computer\HKEY_CLASSES_ROOT\batfile' in the Registry Editor
Create a new key called 'shell' under the 'batfile' key
Create a new key called 'Bat2Exe' under the 'shell' key
Create a new string value called 'Icon' in the key 'Bat2Exe' and enter the path to the 'Bat2Exe.exe' file as the value data
Edit the string value called '(Default)' in the key 'Bat2Exe' and enter 'Convert To Exe' as the value data
Create a new key called 'command' under the 'Bat2Exe' key
Edit the string value called '(Default)' in the key 'command' and enter the path to the 'Bat2Exe.exe' file as the value data
Once these steps are complete any .bat file should have the option to 'Convert To Exe' once the file is right-clicked and 'Show More Options' is pressed
