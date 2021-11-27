# win32-sockets-backdoor
Simple win32 backdoor consisting of a client and a server.

Server:
Spawns a suspended svchost.exe process and injects itself into this and resumes the process.

Supports the following commands:

- Create a new process:
`` start [Program name] ``

- Open a file or website using ShellExecute function:
`` shellexecute [File name] ``

- Shutdown the remote computer:
`` shutdown ``

- Restart the remote computer:
`` restart ``

- Logoff the remote computer:
`` logoff ``

- Force shutdown the remote computer using NtShutdownSystem function:
`` forceshutdown ``

Force restart the remote computer using NtShutdownSystem function:
`` forcerestart ``

- Overwrite the MBR of the remote computer with garbage data, cause the remote computer unable to boot:
`` wipe ``
