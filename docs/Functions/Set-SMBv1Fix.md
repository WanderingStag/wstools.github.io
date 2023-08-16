---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Set-SMBv1Fix

## SYNOPSIS
Enables SMB v1.

## SYNTAX

```
Set-SMBv1Fix [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Turns SMBv1 on.
While this fix action turns SMBv1 on, group policy can turn SMBv1 off, which is counted on.

## EXAMPLES

### EXAMPLE 1
```
Set-SMBv1Fix COMP1
```

Sets the fix action on COMP1.
After the fix action is applied, COMP1 will need to be rebooted.

### EXAMPLE 2
```
Set-SMBv1Fix
```

Sets the fix action on the local computer.
After the fix action is applied, the local computer will need to be rebooted.

## PARAMETERS

### -ComputerName
Specifies the computer or computers

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, CN

Required: False
Position: 1
Default value: "$env:COMPUTERNAME"
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
CREATED: 12/18/2018 09:36:43
LASTEDIT: 12/18/2018 10:25:19
KEYWORDS: fix action, fix, SMB, SMBv1
REQUIRES:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

