---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Install-SCCMUpdate

## SYNOPSIS
Short description

## SYNTAX

```
Install-SCCMUpdate [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Long description

## EXAMPLES

### EXAMPLE 1
```
Install-SCCMUpdate
```

Example of how to use this cmdlet

### EXAMPLE 2
```
Install-SCCMUpdate -PARAMETER
```

Another example of how to use this cmdlet but with a parameter or switch.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, CN

Required: False
Position: 1
Default value: "$env:COMPUTERNAME"
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2023-03-29 22:42:28
Last Edit: 2023-03-29 22:42:28
Other:
Requires:
    -Module ActiveDirectory
    -PSSnapin Microsoft.Exchange.Management.PowerShell.Admin
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

