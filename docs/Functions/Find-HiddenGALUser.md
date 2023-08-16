---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Find-HiddenGALUser

## SYNOPSIS
This function gets all users that are hidden from the GAL.

## SYNTAX

```
Find-HiddenGALUser [[-SearchBase] <String>] [<CommonParameters>]
```

## DESCRIPTION
This function gets all users that are hidden from the Global Address List (GAL) in a domain or you can specify an OU to search.

## EXAMPLES

### EXAMPLE 1
```
Find-HiddenGALUsers -SearchBase "OU=Test,DC=mydomain,DC=com"
```

This function gets all users that are hidden from the GAL in a domain or you can specify an OU to search.

## PARAMETERS

### -SearchBase
Specific OU to search.
If not included, the entire domain will be searched.

```yaml
Type: String
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

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
CREATED: 2014-01-18 02:50:00
LASTEDIT: 2022-09-01 22:30:56
KEYWORDS: Hidden Users, User, Exchange, GAL, Global Address List
REQUIRES:
    ActiveDirectory

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

