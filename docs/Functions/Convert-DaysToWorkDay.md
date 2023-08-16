---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Convert-DaysToWorkDay

## SYNOPSIS

## SYNTAX

```
Convert-DaysToWorkDay [-Days] <Int32> [[-StartDay] <DateTime>] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```
Convert-DaysToWorkDay 1
```

Example of how to use this cmdlet

### EXAMPLE 2
```
Convert-DaysToWorkDay -1
```

Another example of how to use this cmdlet.

## PARAMETERS

### -Days
Enter the amount of days you want to convert.
Must an a positive or negative integer (Ex: 1 or -1).

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDay
Must be in the format yyyy-MM-dd.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: (Get-Date).Date
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: 2021-03-04 18:54:31
Last Edit: 2021-06-20 17:13:33
Keywords:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

