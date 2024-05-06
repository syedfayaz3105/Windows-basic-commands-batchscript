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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-06 161641](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/73579f80-9dbf-4228-b4e9-432a32097e9b)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-06 161714](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/bccaf14e-811a-460d-a6e5-2bff4a0042b9)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```

![Screenshot 2024-05-06 161746](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/c413dbcf-7a3c-4ef9-8539-7b40187b7656)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-06 161819](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/7c4e2d6e-94f0-483b-a141-c4c0b013c72f)



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2024-05-06 161849](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/e97988ce-9933-41bd-beda-8b0aec8ea2f4)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT


![Screenshot 2024-05-06 161934](https://github.com/syedfayaz3105/Windows-basic-commands-batchscript/assets/147144126/4b11f385-4974-4a11-99de-68f982dfd68b)



# RESULT:
The commands/batch files are executed successfully.

