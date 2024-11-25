First we will need to allow the execution of Scripts by changing the execution policy.

```powershell-session
Set-ExecutionPolicy Unrestricted -Scope Process
```

The command will grant the access to execute scripts just in the current terminal, closing it will revoke the changes to the execution policy. You can test those changes using the command:

```powershell-session
Get-ExecutionPolicy -List
```

Now is time to install 'PSWindowsUpdate' a module that allow us to update the system by commands.

```powershell-session
Install-Module PSWindowsUpdate 
```

After that import the module and install the updates:

```powershell-session
Import-Module PSWindowsUpdate 
```

```powershell-session
Install-WindowsUpdate -AcceptAll
```

Then, restart the computer:

```powershell-session
Restart-Computer -Force
```

After that we will install Chocolately Packet Manager using the command:

```powershell-session
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

	This command has three parts, enable the use of scripts, then establish the security protocol TLS in order to connet to the Web page, after that, download and execute the Chocolately installation script.

When we have Chocolately installed, the next step is to update itself using the command:

```powershell-session
choco upgrade chocolatey -y 
```

After that we can instar our apps / software we want.
	If the installation of software gives a vcredist140 error you have to manually install it:
	- https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist
	