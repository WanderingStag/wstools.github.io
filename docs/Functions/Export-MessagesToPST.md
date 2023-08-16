---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Export-MessagesToPST

## SYNOPSIS
This function exports a users mailbox to a pst.

## SYNTAX

```
Export-MessagesToPST [-TargetUserAlias] <String> [[-ExportPath] <String>] [<CommonParameters>]
```

## DESCRIPTION
This function exports a users mailbox to a pst.

## EXAMPLES

### EXAMPLE 1
```
Export-MessagesToPST -TargetUserAlias joe.snuffy
```

Exports joe.snuffy's mailbox to C:\Users\Desktop\joe.snuffy_mailboxyyyyMMddhhmm.pst where yyyyMMddhhmm is
the date and time the mailbox was exported.

### EXAMPLE 2
```
Export-MessagesToPST -TargetUserAlias joe.snuffy -ExportPath "c:\test"
```

Exports joe.snuffy's mailbox to C:\test\joe.snuffy_mailboxyyyyMMddhhmm.pst where yyyyMMddhhmm is the date
and time the mailbox was exported.

## PARAMETERS

### -ExportPath
By default saves to the logged on users desktop.
You can specify where to save the pst to.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: ([System.Environment]::GetFolderPath("Desktop"))
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetUserAlias
Mandatory parameter.
Specify the users alias in Exchange or primary smtp address.

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
CREATED: 01/19/2014 01:20:00
LASTEDIT: 2021-10-13 20:39:47
KEYWORDS: Exchange, Mailbox, PST, export, InTh, Insider Threat
REQUIRES:
    #Requires -PSSnapin Microsoft.Exchange.Management.PowerShell.Admin
    #Requires -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

