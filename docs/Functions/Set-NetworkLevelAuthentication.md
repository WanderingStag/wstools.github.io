---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Set-NetworkLevelAuthentication

## SYNOPSIS

## SYNTAX

```
Set-NetworkLevelAuthentication [[-ComputerName] <String[]>] [-Disable] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```
Set-NetworkLevelAuthentication
```

Will enable network level authentication on the local computer.

### EXAMPLE 2
```
Set-NetworkLevelAuthentication -Disable
```

Will disable network level authentication on the local computer.

### EXAMPLE 3
```
Set-NetworkLevelAuthentication -ComputerName COMP1
```

Will enable network level authentication on the computer COMP1.

## PARAMETERS

### -ComputerName
{{ Fill ComputerName Description }}

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

### -Disable
Specifies to disable Network Level Authentication.
Without this NLA will be enabled.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: 2020-04-18 16:01:02
Last Edit: 2020-04-18 16:01:02
Keywords: Network, NLA, Network Level Authentication, RDP, Remote Desktop
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

