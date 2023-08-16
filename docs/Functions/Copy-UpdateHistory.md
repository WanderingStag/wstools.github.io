---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Copy-UpdateHistory

## SYNOPSIS
Copies the UpdateHistory.csv report to the UHPath config item path.

## SYNTAX

```
Copy-UpdateHistory [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Copies the UpdateHistory.csv report created with Save-UpdateHistory to the UHPath config item path for the
local computer or remote computers.

## EXAMPLES

### EXAMPLE 1
```
Copy-UpdateHistory
```

Example of how to use this cmdlet to copy the UpdateHistory.csv file for the local computer to the UHPath
location.

### EXAMPLE 2
```
Copy-UpdateHistory -ComputerName Server1
```

Example of how to use this cmdlet to copy the UpdateHistory.csv file for the remote computer Server1 to the
UHPath location.

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

### System.String
## NOTES
Author: Skyler Hart
Created: 2022-07-15 22:54:09
Last Edit: 2022-07-15 22:54:09
Other:
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

