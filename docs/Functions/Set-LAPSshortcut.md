---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Set-LAPSshortcut

## SYNOPSIS

## SYNTAX

```
Set-LAPSshortcut [-Path] <String> [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```
Set-LAPSshortcut PublicDesktop
```

Shows how to setup the LAPS shortcut on the Public Desktop.

### EXAMPLE 2
```
Set-LAPSshortcut UserDesktop
```

Shows how to setup the LAPS shortcut on the logged on users desktop.

### EXAMPLE 3
```
Set-LAPSshortcut -Path PublicDesktop
```

Shows how to setup the LAPS shortcut on the Public Desktop.

### EXAMPLE 4
```
Set-LAPSshortcut -Path UserDesktop
```

Shows how to setup the LAPS shortcut on the logged on users desktop.

## PARAMETERS

### -Path
Specifies whether to save to the Public Desktop or the logged on users desktop.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: 2020-05-08 22:34:49
Last Edit: 2021-10-13 20:48:50

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

