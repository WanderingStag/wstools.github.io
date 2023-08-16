---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-HttpHeaderSetting

## SYNOPSIS
Gets the Http Header setting on the current machine.

## SYNTAX

```
Get-HttpHeaderSetting [<CommonParameters>]
```

## DESCRIPTION
Displays the name and value of Http Header settings on the local computer.
Blank entries means the value is not created.

## EXAMPLES

### EXAMPLE 1
```
Get-HttpHeaderSetting
```

Example of how to use this cmdlet.
Will show Http Header settings on the computer.
Will output something similar to this:
Name       Disabled FullPath
----       -------- --------
Parameters        1 HKLM:\SYSTEM\CurrentControlSet\Services\HTTP\Parameters

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2022-11-30 23:43:58
Last Edit: 2022-11-30 23:43:58

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

