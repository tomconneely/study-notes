If there are any problems with knowledge of server admin or netowrking look for these courses on Pluralsight
    Windows Server Administration Fundamentals - Parts 1,2 and 3
    Practiccal Networking

## What is Windows PowerShell
Not only Scripting/CLI
ise cmdlet in PS window will bring up ISE
Server Manager (Server 2012) - there is a PS hisotry at the bottom where you can see the commands that have been run when you make updates in the GUI

## Why you need to know PowerShell
Not going anywhere - MS is all in. 3rd party companies also using it (VMWare/VSphere)
Backed into MS Tools
Automation
Certification - Need to know for exams
Some stuff that can't be done through the GUI

## Demo Notes
Creating CSV file of all services
get-service
get-service | where-object Status -eq 'Stopped' | export-csv c:/test/test.csv

get-service | where-object Status -eq 'Stopped' | select-object Status,Name,Displayname | export-csv c:/test/test.csv

## Demo Notes - Intro to PS Console
Right click upper left corner and click on Properties to change appearance of window
$PSVersionTable cmdlet to get details about PS installed in machine

Blog post on updating Windows 7 machine
http://mikefrobbins.com/2015/01/08/how-to-check-the-powershell-version-and-install-a-new-version/

RSAT = Remote Server Administrative Tools
Can be downloaded for windows 8+