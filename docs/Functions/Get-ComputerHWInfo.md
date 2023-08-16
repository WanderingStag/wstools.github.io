---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-ComputerHWInfo

## SYNOPSIS
Gets hardware information of local or remote computer(s).

## SYNTAX

```
Get-ComputerHWInfo [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Get Manufacturer, Model, Model Version, BIOS vendor, BIOS version, and release date of BIOS update on local
or remote computer.

## EXAMPLES

### EXAMPLE 1
```
Get-ComputerHWInfo
```

Get hardware information for local computer

### EXAMPLE 2
```
Get-ComputerHWInfo COMP1
```

Get hardware information for computer COMP1

## PARAMETERS

### -ComputerName
Used to specify the computer or computers to get hardware information for.

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
AUTHOR: Skyler Hart
CREATED: 3/15/2015 08:49:13
LASTEDIT: 09/21/2017 13:03:30
KEYWORDS: hardware, information, computer
REQUIRES:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

