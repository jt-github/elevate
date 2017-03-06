**Run elevated commands from a regular Windows Command Prompt (no need to Run As AdministratEver had the need to quickly run a command without needing to leave your current Command Prompt window?  Jealous of your Linux friends who have sudo and su?  Well, this isn't anywhere near as good as either of those, but it's a step in the right direction!  Using one of the elevate commands will pop open a new *elevated* PowerShell window so you can quickly run a simple command or even a batch file or PowerShell (PS1) script.ddfasdf

Note that this will, however, activate the User Account Control (UAC) popup to confirm the action, but pressing left-arrow followed by Enter will quickly confirm the action.

Any of the batch files can be run without arguments to simply open an elevated PowerShell window to allow arbitrary commands to be run.

Otherwise, follow the batch file name with a filename<sup>1</sup> or commands and arguments and those will be run in an elevated window.

##elevate.bat
Run a command, batch file or PowerShell file in an elevated PowerShell window, capture the results and spit them out in the initial command window.

##elevatep.bat
Run a command, batch file or PowerShell file in an elevated PowerShell window and then pause (does not capture any results).

##elevatex.bat
Run command, batch file or PowerShell file in an elevated PowerShell window and keep the PowerShell window open for more work.

###Example:
`elevate dir C:\users\some_user_you_dont_normally_have_access_to`

<sup>1</sup> Any filenames must be fully qualified since the PowerShell window opens as Administrator in the C:\Windows\System32 folder.
