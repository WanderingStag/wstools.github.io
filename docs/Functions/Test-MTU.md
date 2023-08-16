---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Test-MTU

## SYNOPSIS
Finds the MTU size for packets to a remote computer.

## SYNTAX

```
Test-MTU [[-RemoteAddress] <String[]>] [[-BufferSizeMax] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Will find the point where packets don't fragment (MTU) to a remote source, which defaults to the computers logon server if an address isn't specified.

## EXAMPLES

### EXAMPLE 1
```
Test-MTU
```

Example of how to use this cmdlet.

### EXAMPLE 2
```
Test-MTU www.wanderingstag.com
```

Shows how to test the MTU to the website www.wanderingstag.com.

### EXAMPLE 3
```
Test-MTU COMP1,www.wanderingstag.com
```

Shows how to test the MTU to the computer COMP1 and the website www.wanderingstag.com.

### EXAMPLE 4
```
Test-MTU COMP1 1272
```

Shows how to test the MTU to the computer COMP1, the max buffer size (MTU) will start at 1272.

## PARAMETERS

### -BufferSizeMax
Allows you to specify the highest MTU to test.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 1500
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoteAddress
Specifies the name or IP of one or more remote computers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Host, Name, Computer, ComputerName, TestAddress

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2022-11-22 21:27:58
Last Edit: 2022-11-22 23:06:11
Other:
Requires:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

