---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-LockedOutLocation

## SYNOPSIS
This function will locate the computer that processed a failed user logon attempt which caused the user account to become locked out.

## SYNTAX

```
Get-LockedOutLocation [-Identity] <String> [<CommonParameters>]
```

## DESCRIPTION
This function will locate the computer that processed a failed user logon attempt which caused the user account to become locked out.
The locked out location is found by querying the PDC Emulator for locked out events (4740).
The function will display the BadPasswordTime attribute on all of the domain controllers to add in further troubleshooting.

## EXAMPLES

### EXAMPLE 1
```
Get-LockedOutLocation -Identity Joe.Davis
```

This example will find the locked out location for Joe Davis.

## PARAMETERS

### -Identity
{{ Fill Identity Description }}

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
This function is only compatible with an environment where the domain controller with the PDCe role to be running Windows Server 2008 SP2 and up.
The script is also dependent the ActiveDirectory PowerShell module, which requires the AD Web services to be running on at least one domain controller.
Author:Jason Walker
Last Modified: 3/20/2013

## RELATED LINKS
