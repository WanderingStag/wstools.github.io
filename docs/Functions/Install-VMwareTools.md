---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Install-VMwareTools

## SYNOPSIS
Will install VMware tools on one or more computers.

## SYNTAX

```
Install-VMwareTools [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Installes VMware Tools from the C:\Patches\VMware directory.
Uses config file to determine network path to copy to the local computer first.
On remote computers, install file will need to already exist (use Copy-VMwareTools).

## EXAMPLES

### EXAMPLE 1
```
Install-VMwareTools
```

Will install VMware Tools from setup file in C:\Patches\VMwareTools.

### EXAMPLE 2
```
Install-VMwareTools -ComputerName COMP1,COMP2
```

Will install VMware Tools from setup file in C:\Patches\VMwareTools on COMP1 and COMP2.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers to install VMware Tools on.

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

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: 2022-12-16 22:04:04
Last Edit: 2022-12-16 22:04:04
Keywords:
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

