# elevateddfasfdasdf
Run elevated commands from a regular Windows Command Prompt (no need to Run As Administrator!)
Note that this does, however, activate the User Account Control (UAC) popup to confirm the action, but a quick left-arrow followed by Enter will quickly confirm the action.

Any of the batch files can be run without arguments to simply open an elevated PowerShell window to allow arbitrary commands to be run.

Otherwise, follow the batch file name with any commands and arguments and those will be run in an elevated window.

elevate.bat
Run a command, batch file or PowerShell file in an elevated PowerShell window, capture the results and spit them out in the initial command window.

elevatep.bat
Run a command, batch file or PowerShell file in an elevated PowerShell window and then pause (does not capture any results).

elevatex.bat
Run command, batch file or PowerShell file in an elevated PowerShell window and keep the PowerShell window open for more work.

Example:
elevate dir C:\users\some_user_you_dont_normally_have_access_to
