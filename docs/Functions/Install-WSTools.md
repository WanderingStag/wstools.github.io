---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Install-WSTools

## SYNOPSIS
Installs/copies the WSTools PowerShell module to a remote computer.

## SYNTAX

```
Install-WSTools [[-ComputerName] <String[]>] [[-MaxThreads] <Int32>] [[-SleepTimer] <Object>]
 [[-MaxResultTime] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Copies the WSTools module from the location specified in the WSTools config file (config.ps1) for UpdatePath to the C:\Program Files\WindowsPowerShell\Modules\WSTools folder on the remote computer.

## EXAMPLES

### EXAMPLE 1
```
Install-WSTools COMPNAME
```

How to install the WSTools PowerShell module on the remote computer COMPNAME.

### EXAMPLE 2
```
Install-WSTools -ComputerName COMPNAME1,COMPNAME2
```

How to install the WSTools PowerShell module on the remote computers COMPNAME1 and COMPNAME2.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, CN, common name

Required: False
Position: 1
Default value: $env:COMPUTERNAME
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

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
Author: Skyler Hart
Created: 2018-06-13 14:17:09
Last Edit: 2022-02-19 22:56:29
Keywords:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

