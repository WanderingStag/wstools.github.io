---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Repair-DuplicateSusClientID

## SYNOPSIS
Removes SusClientID registry key on the local or remote computer.

## SYNTAX

```
Repair-DuplicateSusClientID [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
When creating a computer from a template (virtual disc) the SusClientID isn't changed and will result in WSUS only having one object for all the computers created.
This function clears the SusClientID from the registry on the local or remote computer(s) so when syncing with WSUS a new SusClientID will be created.
The first initial sync with WSUS typically fails.
It may take several minutes for the computer to sync appropriately with WSUS.

## EXAMPLES

### EXAMPLE 1
```
Repair-DuplicateSusClientID
```

Example of how to use this cmdlet to fix a duplicate SusClientID on the local computer.

### EXAMPLE 2
```
Repair-DuplicateSusClientID -ComputerName Server1
```

Another example of how to use this cmdlet but with the ComputerName parameter.
In this example, Server1 is a remote computer.

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
Created: 2022-07-15 21:05:27
Last Edit: 2022-07-15 21:05:27
Other:
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

