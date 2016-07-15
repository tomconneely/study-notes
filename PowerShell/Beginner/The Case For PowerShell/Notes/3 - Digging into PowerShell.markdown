## Using Get-Command to Discover Commands
    To discover cmdlets use Get-Command
        get-command *printer*
        gcm *printer* alias
        Both would should any cmdlets with printer in the name
        Where-Object -> Where
        Sort-Object -> Sort
    Help can be updated

## Remote Control with PowerShell
    Can use invoke-command cmdlet to run scriptblock on other pcs
    invoke-command -computername pc1, pc2 -scriptblock {...}
    invoke-command -computername (type c:\pcs.text) -scriptblock {...}  List of pcs, 1 on each line
    invoke-command -computername (get-adcomputer -filter *).name -scriptblock {...}     All AD computers in network

## The PowerShell Pipeline
    The "|" symbol
    Allows us to take the output of 1 cmdlet and put it into the input of another cmdlet
    Pipeline transfers .NET, CIM and COM objects
        Passes objects not text when piped
    Use a cmdlet that finds things
        Users that have not logged in in 90 days
    And pipe it to a cmdlet that does things
        Disable account

    Any PowerShell cmdlet that could do any damage has the option -whatif
    Gives response that says what it would have done without the -whatif so you can check if correct

##Examples of Where PowerShell has Helped
    PowerGUI - Look into this

## Summary
help@minasi.com
Twitter: mminasi