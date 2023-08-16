---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Copy-UserProfile

## SYNOPSIS

## SYNTAX

```
Copy-UserProfile [-User] <String> [[-ComputerName] <String[]>] [-Destination <String>] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ComputerName
Enter one or more computer names separated by commas.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, CN

Required: False
Position: 2
Default value: "$env:COMPUTERNAME"
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Destination
Enter destination folder path as UNC unless a local path.
Ex: E:\ESI\10-001 or \\\\COMP\e$\ESI\10-001

```yaml
Type: String
Parameter Sets: (All)
Aliases: Dest, DestinationFolder, DestFolder

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -User
Enter user name.
Ex: "1234567890A" without quotes

```yaml
Type: String
Parameter Sets: (All)
Aliases: Username, SamAccountName

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
CREATED: 04/06/2020 19:39:42
LASTEDIT: 04/06/2020 20:10:59
KEYWORDS:
REQUIRES:
    -Version 3.0
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

