---
external help file: WSTools-help.xml
Module Name: WSTools
online version:
schema: 2.0.0
---

# Get-ExchangeLastLoggedOnUser

## SYNOPSIS

## SYNTAX

```
Get-ExchangeLastLoggedOnUser [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
LASTEDIT: 08/18/2017 20:58:33
KEYWORDS:
REQUIRES:
    #Requires -Version 3.0
    #Requires -Modules ActiveDirectory
    #Requires -PSSnapin Microsoft.Exchange.Management.PowerShell.Admin
    #Requires -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io

Get-ADUser -Filter {EmailAddress -like "*"} -properties * | select EmailAddress | Export-Csv .\users.csv -NoTypeInformation]()

