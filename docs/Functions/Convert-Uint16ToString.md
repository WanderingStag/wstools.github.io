---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Convert-Uint16ToString

## SYNOPSIS
Converts uin16 arrays to a readable string.

## SYNTAX

```
Convert-Uint16ToString [[-Members] <UInt16[]>] [<CommonParameters>]
```

## DESCRIPTION
Take the members from a uint16 array and converts it to a user friendly string.

## EXAMPLES

### EXAMPLE 1
```
Convert-Uint16ToString $uint16array
```

Converts the uint16 array in the $uint16array variable.

### EXAMPLE 2
```
Convert-Uint16ToString ((Get-CimInstance WmiMonitorID -Namespace root/WMI)[0] | Select-Object -ExpandProperty SerialNumberID)
```

Converts the SerialNumberID of the first monitor to a readable format.

## PARAMETERS

### -Members
Takes the array members for a uint16 array.

```yaml
Type: UInt16[]
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

### System.uint16
## OUTPUTS

### System.String
## NOTES
Author: Skyler Hart
Created: 2023-02-11 01:02:00
Last Edit: 2023-02-11 01:02:00

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

