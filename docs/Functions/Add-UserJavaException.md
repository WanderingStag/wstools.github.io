---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Add-UserJavaException

## SYNOPSIS
Adds Java exception.

## SYNTAX

```
Add-UserJavaException [-URI] <String> [<CommonParameters>]
```

## DESCRIPTION
Will add a website entry to $env:USERPROFILE\AppData\LocalLow\Sun\Java\Deployment\security\exception.sites.

## EXAMPLES

### EXAMPLE 1
```
Add-UserJavaException https://wanderingstag.github.io
```

Example of how to use this cmdlet

## PARAMETERS

### -URI
Specifies the URI of the website you want to add to the exception.sites file.
Must be in the
format https://wanderingstag.github.io.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Site, URL, Address, Website

Required: True
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

### No output
## NOTES
Author: Skyler Hart
Created: 2019-03-20 10:40:11
Last Edit: 2021-12-20 00:15:00

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

