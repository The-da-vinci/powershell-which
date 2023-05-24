# Powershell-which

`PowerShell-which` is a handy PowerShell function that emulates the `which` command in Unix/Linux environments. It aids users in locating the executable path for a specific command within their current PowerShell session. This function leverages the `Get-Command` cmdlet to identify the command and fetches the executable path using the `Definition` property.

## Installation

Setting up `PowerShell-which` in your PowerShell environment involves adding the function to your PowerShell profile file. Here's how you can do it:

1. Open PowerShell and run the following command to find the path of your profile file:
   `$profile.CurrentUserAllHosts `
2. If the file does not exist, create it by running the following command:
   `New-Item -ItemType File -Path $profile.CurrentUserAllHosts -Force`
3. Open the profile file in a text editor by running the following command:
   `notepad $profile.CurrentUserAllHosts`
4. Add the `powershell-which` function to the profile file by copying and pasting the function code into the file.
5. Save the profile file and close the text editor.
   Now, `powershell-which` function is ready for use in your PowerShell sessions and scripts.

.

## Usage

```
which <command>
```

Example:

```
which python
```

This will return the path of the `python.exe` executable.
