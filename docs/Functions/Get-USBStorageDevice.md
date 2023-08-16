---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-USBStorageDevice

## SYNOPSIS
Shows USB storage devices that have connected to a computer.

## SYNTAX

```
Get-USBStorageDevice [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Shows USB storage devices that have connected to a local or remote computer.
Limitations apply.
Only shows devices that are listed in the registry.
Sometimes, depending on the computer that is only the most recent device.

## EXAMPLES

### EXAMPLE 1
```
Get-USBStorageDevice
```

Example of how to use this cmdlet on a local computer.

### EXAMPLE 2
```
Get-USBStorageDevice -ComputerName COMP1
```

Shows the USB storage devices that have connected to the remote computer COMP1.

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
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: Sometime before 8/7/2017
Last Edit: 2021-06-28 22:46:02
Keywords:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

