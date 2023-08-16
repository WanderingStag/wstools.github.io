---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-InstalledProgram

## SYNOPSIS
Displays installed programs on a computer.

## SYNTAX

```
Get-InstalledProgram [[-ComputerName] <String[]>] [[-Property] <String[]>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Displays a list of installed programs on a local or remote computer by querying the registry.

## EXAMPLES

### EXAMPLE 1
```
Get-InstalledProgram
```

Shows the installed programs on the local computer.

### EXAMPLE 2
```
Get-InstalledProgram -ComputerName COMPUTER1
```

Shows the installed programs on the remote computer COMPUTER1.

### EXAMPLE 3
```
Get-InstalledProgram -ComputerName COMPUTER1,COMPUTER2
```

Shows the installed programs on the remote computers COMPUTER1 and COMPUTER2.

### EXAMPLE 4
```
Get-InstalledProgram (gc C:\Temp\computers.txt)
```

Shows the installed programs on the remote computers listed in the computers.txt file (each computer name on a new line.)

### EXAMPLE 5
```
Get-InstalledProgram COMPUTER1 -Property InstallSource
```

Shows the installed programs on the remote computer COMPUTER1 and also shows the additional property InstallSource from the registry.

### EXAMPLE 6
```
Get-InstalledProgram COMPUTER1,COMPUTER2 -Property InstallSource,Comments
```

Shows the installed programs on the remote computers COMPUTER1 and COMPUTER2.
Also shows the additional properties InstallSource and Comments from the registry.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, DNSHostName, Computer

Required: False
Position: 1
Default value: $env:COMPUTERNAME
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Property
Will add additional properties to pull from the Uninstall key in the registry.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Skyler Hart
Created: Sometime prior to 2017-08
Last Edit: 2020-08-19 23:03:32
Keywords: Software, Programs, management

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

