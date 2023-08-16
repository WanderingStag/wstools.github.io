---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Save-MaintenanceReport

## SYNOPSIS

## SYNTAX

```
Save-MaintenanceReport [[-Days] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Days
{{ Fill Days Description }}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: ((Get-Date -Format yyyyMMdd) - ((Get-Date -Format yyyyMMdd).Substring(0,6) + "01"))
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: 2020-06-16 14:39:04
Last Edit: 2023-03-22 08:26:11
Keywords:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

