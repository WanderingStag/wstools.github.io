---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Import-MOF

## SYNOPSIS

## SYNTAX

```
Import-MOF [-Path] <String> [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```
Import-MOF C:\Example\windows10.mof
```

Example of how to use this cmdlet.

### EXAMPLE 2
```
New-WMIFilter 'C:\setup\GPOs\WMIs\Google Chrome\Google Chrome.mof'
```

Example of how to use this cmdlet.

### EXAMPLE 3
```
Import-MOF -Path C:\Example\virtualservers.mof
```

Another example of how to use this cmdlet but with a parameter or switch.

## PARAMETERS

### -Path
Specifies the path to the mof file intended to import.

```yaml
Type: String
Parameter Sets: (All)
Aliases: mof, Name, File

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
Created: 10/27/2017 15:54:18
Last Edit: 2020-05-08 20:30:19
Keywords:
Requires:
    -Module ActiveDirectory

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

