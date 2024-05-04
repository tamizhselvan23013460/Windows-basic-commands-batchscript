# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/590a728d-d559-41dc-952b-e6ca39d351a8)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/a7f9c654-8258-4be6-85ac-0d302c19a87e)

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/23fc2e3e-ff15-4ef4-8f5a-aa74aa29873d)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/b32c5ce8-6574-4b46-9b0f-ad303f5c5466)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/f98b8267-6985-4369-8ce1-72080b671de9)

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/14374518-37aa-411e-89cc-8c4afb106cae)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/91fa0b29-7527-48a2-9137-21dbe0033cf8)


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

![image](https://github.com/tamizhselvan23013460/Windows-basic-commands-batchscript/assets/150231370/bfb2c103-6329-4b73-bae8-3fe0fcba8293)

# RESULT:
The commands/batch files are executed successfully.

