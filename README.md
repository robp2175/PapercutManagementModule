PapercutManagementModule
========================

This is a fork of jeffpatton1971's PowerShell module for working with the Papercut API. He was missing some cmdlets I needed for my application of PapercutMF, inpartcular adding Shared Accounts and there respective properties. I plan to keep adding the missing cmdlets as I go so that this is eventually complete. 

You will need to have Visual Studio installed, I use version 2013.

Open the project file and build the project, which will result in a PapercutManagement.dll file in PapercutManagement\bin\Release.

You might also need to add xmlrpcnet reference from NuGet (xmlrpcnet.3.0.0.266). However, I have included the dll in packages. 

#How to use:
* Import-Module .\PapercutManagement.dll
* To see available cmdlets: Get-Command -Module PapercutManagement
* Connect to Papercut Server: Connect-pcutServer -ComputerName PcutServerName -authToken adminPassword
  * IP of connecting machine must be added to papercut server and API enabled. Options > Advanced > Allowed XML Web Services callers.


