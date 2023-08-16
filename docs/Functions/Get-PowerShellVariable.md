---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-PowerShellVariable

## SYNOPSIS
Will show env: and PowerShell variable active in session.

## SYNTAX

```
Get-PowerShellVariable [[-Name] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Gets environment variables and the active PowerShell variables in the current session and shows their values.

## EXAMPLES

### EXAMPLE 1
```
Get-PowerShellVariable
```

Example of how to use this cmdlet.

### EXAMPLE 2
```
Get-PowerShellVariable -Name ErrorActionPreference
```

Will show what the value is for $ErrorActionPreference.

### EXAMPLE 3
```
Get-PowerShellVariable -Name ErrorActionPreference,OneDriveConsumer
```

Will show what the value is for $ErrorActionPreference and $env:OneDriveConsumer.

## PARAMETERS

### -Name
To filter for a specific variable.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
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
Created: 2022-09-22 23:29:51
Last Edit: 2022-09-22 23:29:51
Other:
Requires:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

