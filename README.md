# SCCM

## Adding Prequisites files before installing SCCM/MECM Current branch 2403
 Scripts added frequently 

'''
# .NET Features
Install-WindowsFeature -Name NET-Framework-Features
Install-WindowsFeature -Name NET-Framework-Core
Install-WindowsFeature -Name NET-Framework-45-Features
Install-WindowsFeature -Name NET-Framework-45-Core
Install-WindowsFeature -Name NET-Framework-45-ASPNET
Install-WindowsFeature -Name NET-WCF-Services45
Install-WindowsFeature -Name NET-WCF-HTTP-Activation45
Install-WindowsFeature -Name NET-WCF-TCP-PortSharing45

# Install IIS Web Server Role
Install-WindowsFeature -Name Web-Server -IncludeManagementTools
Install-WindowsFeature -Name Web-WebServer

# Application Development
Install-WindowsFeature -Name Web-ISAPI-Ext

# Security
Install-WindowsFeature -Name Web-Windows-Auth

# Management Tools
Install-WindowsFeature -Name Web-Mgmt-Tools
Install-WindowsFeature -Name Web-Mgmt-Console
Install-WindowsFeature -Name Web-Mgmt-Compat
Install-WindowsFeature -Name Web-Metabase
Install-WindowsFeature -Name Web-WMI

# Install Background Intelligence Transfer Service (BITS)
Install-WindowsFeature -Name BITS
Install-WindowsFeature -Name BITS-IIS-Ext
'''

Other files and scripts will be added accordingly

echo "# SCCM" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/SaraBinthAjmal/SCCM.git
git push -u origin main

git remote add origin https://github.com/SaraBinthAjmal/SCCM.git
git branch -M main
git push -u origin main