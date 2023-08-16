---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-NonSmartCardRequiredUser

## SYNOPSIS
Displays users in domain with SmartCardRequired attribute set to false.

## SYNTAX

```
Get-NonSmartCardRequiredUser [[-Name] <String>] [<CommonParameters>]
```

## DESCRIPTION
Displays all users in the domain with SmartCardRequired attribute on account set to false.

## EXAMPLES

### EXAMPLE 1
```
Get-NonSmartCardRequiredUser
```

Example of how to use this cmdlet

## PARAMETERS

### -Name
{{ Fill Name Description }}

```yaml
Type: String
Parameter Sets: (All)
Aliases: User

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### System.Array
## NOTES
Author: Skyler Hart
Created: 2023-05-02 17:16:53
Last Edit: 2023-05-02 17:16:53
Requires:
    -Module ActiveDirectory

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

