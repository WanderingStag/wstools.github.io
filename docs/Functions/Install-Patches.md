---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Install-Patches

## SYNOPSIS
Will install patches in the local patches folder.

## SYNTAX

```
Install-Patches [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Installes patches in the LocalPatches config setting path (default is C:\Patches.)

## EXAMPLES

### EXAMPLE 1
```
Install-Patches
```

Will install patches in the LocalPatches config setting path (default is C:\Patches.)

### EXAMPLE 2
```
Install-Patches -ComputerName COMP1,COMP2
```

Will install patches in the LocalPatches config setting path (default is C:\Patches) on COMP1 and COMP2.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers to install patches on.

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
Created: 2017-03-25 08:30:23
Last Edit: 2021-08-12 00:36:14
Keywords:
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

