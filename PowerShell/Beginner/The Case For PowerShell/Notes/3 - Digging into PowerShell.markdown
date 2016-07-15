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

##Examples of Where PowerShell has Helped


## Summary