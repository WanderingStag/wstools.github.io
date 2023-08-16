---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Clear-ImproperProfileCopy

## SYNOPSIS
Clears Application Data folder that was improperly copied which happens when copy and pasting a profile.

## SYNTAX

```
Clear-ImproperProfileCopy [-Source] <String> [-Destination] <String> [<CommonParameters>]
```

## DESCRIPTION
Copies nested Application Data folders to a higher level (by default to C:\f2) and deletes them.

## EXAMPLES

### EXAMPLE 1
```
Clear-ImproperProfileCopy -Source \\fileserver\example\user -Destination E:\f2
```

Clears nested Application Data folders from \\\\fileserver\example\user.
Uses E:\f2 as the folder for
clearing.

### EXAMPLE 2
```
Clear-ImproperProfileCopy E:\temp\Profile E:\f2
```

Clears nested Application Data folders from E:\temp\Profile.
Uses E:\f2 as the folder for clearing.

## PARAMETERS

### -Destination
Specifies the folder that is used to copy the nested folders to and deletes them.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Source
Specifies the folder that contains the Application Data folder causing issues.

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
CREATED: 06/11/2016 20:37:14
LASTEDIT: 2020-04-15 21:54:21
KEYWORDS: user, profile, app data, application data, cleanup, clear, improper

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

