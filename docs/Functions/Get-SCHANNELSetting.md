---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-SCHANNELSetting

## SYNOPSIS
Gets the SCHANNEL settings on the current machine.

## SYNTAX

```
Get-SCHANNELSetting [[-Name] <String>] [<CommonParameters>]
```

## DESCRIPTION
Displays the name and value of SCHANNEL settings on the local computer.
Blank entries means the value is not created.

## EXAMPLES

### EXAMPLE 1
```
Get-SCHANNELSetting
```

Example of how to use this cmdlet.
Will show all SCHANNEL settings on the computer.
Will output something similar to this:
Name                                 DisabledByDefault    Enabled FullPath
----                                 -----------------    ------- --------
Ciphers\DES 56/56                                               0 HKLM:\SYSTEM\CurrentControlSet\Control\SecurityPro...
Ciphers\NULL                                                    0 HKLM:\SYSTEM\CurrentControlSet\Control\SecurityPro.

### EXAMPLE 2
```
Get-SCHANNELSetting -Name Ciphers
```

Will show all the Ciphers configured in the SCHANNEL registry settings.

### EXAMPLE 3
```
Get-SCHANNELSetting -Name "TLS 1.0"
```

Will show all the TLS 1.0 SCHANNEL registry settings configured on the computer.

## PARAMETERS

### -Name
Used to specify the name of a SCHANNEL setting to display.
Uses matching.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Path

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
Created: 2022-09-05 00:24:25
Last Edit: 2022-09-05 00:56:53

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

