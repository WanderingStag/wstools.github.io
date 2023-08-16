---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-OperatingSystem

## SYNOPSIS
Gets Operating System information

## SYNTAX

```
Get-OperatingSystem [[-ComputerName] <String[]>] [-Registry] [<CommonParameters>]
```

## DESCRIPTION
Gets Operating System information via WMI query (Default) or Registry query (Switch.) Determines whether the computer is 32-bit or 64-bit, the Operating System name, and the OS Build number.

## EXAMPLES

### EXAMPLE 1
```
Get-OperatingSystem
```

Gets Operating System information for the local computer

### EXAMPLE 2
```
Get-OperatingSystem -Registry
```

Gets Operating System information for the local computer via Registry query instead os WMI query

### EXAMPLE 3
```
Get-OperatingSystem -ComputerName SERVER1
```

Gets Operating System information for computer SERVER1

### EXAMPLE 4
```
Get-OperatingSystem -ComputerName (gc c:\complist.txt) -Registry
```

Gets Operating System information for all computers listed in c:\complist.txt via Registry queries

## PARAMETERS

### -ComputerName
Specify computer or computer names to query

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

### -Registry
Use Registry queries instead of WMI queries

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
CREATED: 06/06/2015 20:11:37
LASTEDIT: 2021-11-26 17:02:59
KEYWORDS: Operating System, OS
REMARKS: For local computer it can be ran as user.
For remote computers, it needs to be ran as a user who has administrative rights on the remote computer.

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

