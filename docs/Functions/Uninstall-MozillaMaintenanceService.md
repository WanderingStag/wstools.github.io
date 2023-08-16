---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Uninstall-MozillaMaintenanceService

## SYNOPSIS

## SYNTAX

```
Uninstall-MozillaMaintenanceService [[-ObjectList] <String[]>] [[-MaxThreads] <Int32>] [[-SleepTimer] <Object>]
 [[-MaxResultTime] <Object>] [<CommonParameters>]
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

### -MaxResultTime
{{ Fill MaxResultTime Description }}

```yaml
Type: Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 1200
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxThreads
{{ Fill MaxThreads Description }}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 5
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectList
Enter one or more computer names separated by commas.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, CN, ComputerName

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -SleepTimer
{{ Fill SleepTimer Description }}

```yaml
Type: Object
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 200
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
CREATED: 08/01/2019 16:36:26
LASTEDIT: 08/01/2019 16:36:26
KEYWORDS:
REQUIRES:
    #Requires -Version 3.0
    #Requires -Modules ActiveDirectory
    #Requires -PSSnapin Microsoft.Exchange.Management.PowerShell.Admin
    #Requires -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

