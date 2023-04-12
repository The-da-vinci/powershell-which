# Powershell-which

`powershell-which` is a function that finds the path of the executable for a given command in the current PowerShell session, similar to the `which` command in Unix/Linux systems. It uses the `Get-Command` cmdlet to search for the command and returns the path using the `Definition` property of the output.

## Installation

To use `powershell-which`, you will need to add the function to your PowerShell profile file. To do this, follow these steps:

1. Open PowerShell and run the following command to find the path of your profile file:
   `$profile.CurrentUserAllHosts `
2. If the file does not exist, create it by running the following command:
   `New-Item -ItemType File -Path $profile.CurrentUserAllHosts -Force`
3. Open the profile file in a text editor by running the following command:
   `notepad $profile.CurrentUserAllHosts`
4. Add the `powershell-which` function to the profile file by copying and pasting the function code into the file.
5. Save the profile file and close the text editor.
   Now, you can use the `powershell-which` function in your PowerShell sessions and scripts.

## Usage

```
which <command>
```

Example:

```
which python
```

This will return the path of the `python.exe` executable.
