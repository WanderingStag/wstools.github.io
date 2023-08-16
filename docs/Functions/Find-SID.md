---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Find-SID

## SYNOPSIS
This function finds what Active Directory object the specified SID belongs to.

## SYNTAX

```
Find-SID [-SID] <String> [<CommonParameters>]
```

## DESCRIPTION
This function finds what Active Directory object the specified SID belongs to.

## EXAMPLES

### EXAMPLE 1
```
Find-SID "S-1-5-21-1454471165-1004335555-1606985555-5555"
```

Finds what Active Directory object the specified SID belongs to.

## PARAMETERS

### -SID
Mandatory parameter.
Specify the SID you want to search for.

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
AUTHOR: Skyler Hart
CREATED: 2014-01-19 01:45:00
LASTEDIT: 08/15/2018 22:47:26
KEYWORDS: SID

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

