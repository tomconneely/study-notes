Notes from Pluralsight course in the What Are Containers? section

Applications used to run on individual servers
Server procurement meant getting big and fast servers even if they were excessive

## Hello VMWare
Instead of dedicating one server to one app, now you could run multiple apps on one server

Not a perfect solution

## VMWarts
On a server you have CPU, RAM and disk resources
For hypervisor, it requires a separate VM for each app
VM is slice of server
Each VM requires OS (Windows/Linux) in order to run.
Each OS uses CPU, RAM and disk resources
Each OS normally requires licences
They also require admin time (security, antivirus, etc)


## Containers
Same 4 apps but have 1 OS at the bottom
Each app runs in its own container
Containers are normally smaller and more efficient than hypervisor