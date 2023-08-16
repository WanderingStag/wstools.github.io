---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Clear-DirtyShutdown

## SYNOPSIS
Clears dirty shutdown registry key.

## SYNTAX

```
Clear-DirtyShutdown [[-ComputerName] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Clears the registry key that prompts you to enter a reason the computer/server was shutdown, even after a
clean shutdown.

## EXAMPLES

### EXAMPLE 1
```
Clear-DirtyShutdown
```

Will clear a dirty shutdown that causes the shutdown tracker to appear.

### EXAMPLE 2
```
Clear-DirtyShutdown -ComputerName COMP1
```

Will clear the dirty shutdown on COMP1.
You must have admin rights on the remote computer.

## PARAMETERS

### -ComputerName
Specifies the name of one or more computers.

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

### System.String
## OUTPUTS

### No output
## NOTES
Author: Skyler Hart
Created: 2020-05-08 17:54:09
Last Edit: 2021-12-19 23:58:28
Requires -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

