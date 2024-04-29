# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript      
NAME:N.NAVYA SREE    
REG.NO:212223040138

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/a5550631-3a50-4130-affb-49a31e1e71ed)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/4294b8e0-0ce5-4bf1-9c1c-0b307f86aeaf)

![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/f9922445-c18e-49d1-a57b-5cc418ace200)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab


![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/6854c2bc-3baa-435a-a842-044c44e2d0b9)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/fcdd49c2-5cf7-4ea8-a498-aadfab0bdd7f)


![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/c98ae56b-53da-43f6-a881-ee76249092b2)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents


![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/88a1caa1-6d10-43c0-bd83-230aea710a1b)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```



## OUTPUT


![image](https://github.com/KUSHALI104/Windows-basic-commands-batchscript/assets/150231135/122fe64e-8b58-431c-8b3c-3a7f6661daf3)





# RESULT:
The commands/batch files are executed successfully.

