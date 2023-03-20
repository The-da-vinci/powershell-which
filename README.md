# pwsh-which

`pwsh-which` is a PowerShell function that returns the path of the executable that would be executed in the current environment if the given command is executed. This is similar to the `which` command in Unix/Linux systems.

## Installation

To use `pwsh-which`, you will need to add the function to your PowerShell profile file. To do this, follow these steps:

1. Open PowerShell and run the following command to find the path of your profile file:
   `$profile.CurrentUserAllHosts `
2. If the file does not exist, create it by running the following command:
   `New-Item -ItemType File -Path $profile.CurrentUserAllHosts -Force`
3. Open the profile file in a text editor by running the following command:
   `notepad $profile.CurrentUserAllHosts`
4. Add the `pwsh-which` function to the profile file by copying and pasting the function code into the file.
5. Save the profile file and close the text editor.
   Now, you can use the `pwsh-which` function in your PowerShell sessions and scripts.

## Usage
```
which <command>
```
Example:
```
which python
```
This will return the path of the `python.exe` executable.
