## PowerShell Cmdlet Structure
    All PowerShell cmdlets have name like verb-noun
        Verbs = new, get, connect, set, remove, select
        Verbs are controlled but cmdlets aren't. Anyone can write cmdlets
    The nouns come from the product group that controls whatever you're trying to administer
        Process, Service, Computer
        Get-Process = Like Task Manager, shows all running processes
        ADUser
    Nouns are always singular
        Get lets you list things

## Top PowerShell Verbs
    4 Big PowerShell Verbs
    New = Create something new
        No cmdlet starts with create
    Get = Show or list
        get-vm would show all VMs on HyperV server
    Set = Lets you change some characteristic
        set-vm would let you rename it, change RAM, etc.
    Remove = Delete
        remove-vm would delete a VM

    Other verbs are ass, clear, test, measure, rename
    Can see all verbs using cmdlet get-verb

    Reusable Information
        To rename a VM from WEBVM to VM1
            rename-vm -name "WebVM" -newname "VM1"
        To rename pc24 to accountingpc
            rename-computer -name "pc24" -newname "accountingpc"
        Same structure/syntax

    PowerShell mainly soesn't care about case (99.9% of cases)
    Tab completion functionality
    Shift + Tab takes you back

## Shortening PowerShell Commands
    Can use aliases to shorten commands
        import-module becomes ipmo

## Examples of PowerShell