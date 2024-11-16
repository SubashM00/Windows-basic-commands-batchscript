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
![image](https://github.com/user-attachments/assets/151700e0-81f9-4795-8191-3dabaef32263)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/1032efe2-11fd-40a8-9beb-bb7ce40f93b9)
```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/ecd970fe-740e-4f80-aef0-31a7aabc5d14)
List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/e21a8591-ae47-485c-8d9c-5750da8c04a2)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/82eaead6-373e-476b-844f-1abe95954784)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/6b03fba9-5695-4d18-b96a-791f882ad9f6)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```
![image](https://github.com/user-attachments/assets/acc9191b-d92d-4bbd-b424-71035ddae0df)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

# COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![image](https://github.com/user-attachments/assets/e17455fc-8667-4bcf-ade5-148b98cb244b)

# COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/user-attachments/assets/9f89b5f8-8e8b-4978-9368-5b6643e0455e)



# RESULT:
The commands/batch files are executed successfully.

