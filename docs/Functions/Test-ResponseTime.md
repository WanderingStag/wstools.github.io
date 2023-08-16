---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Test-ResponseTime

## SYNOPSIS
Finds the response time of a remote computer.

## SYNTAX

```
Test-ResponseTime [[-RemoteAddress] <String[]>] [[-ThrottleLimit] <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Will find average, minimum, and maximum response times (from four pings) of a remote computer, which defaults to the computers logon server if an address is not specified.

## EXAMPLES

### EXAMPLE 1
```
Test-ResponseTime
```

Example of how to use this cmdlet.

### EXAMPLE 2
```
Test-ResponseTime www.wanderingstag.com
```

Shows how to test the response time to the website www.wanderingstag.com.

### EXAMPLE 3
```
Test-ResponseTime COMP1,www.wanderingstag.com
```

Shows how to test the response time to the computer COMP1 and the website www.wanderingstag.com.

### EXAMPLE 4
```
Test-MTU COMP1,COMP2,COMP3,www.wanderingstag.com -ThrottleLimit 2
```

Shows how to test the response times to multiple computers, the test will be performed against two of the computers at a time.

## PARAMETERS

### -RemoteAddress
Specifies the name of one or more remote computers.

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

### -ThrottleLimit
Allows you to specify the most remote computers that will be tested at a time, defaults to 5.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2023-02-01 22:51:01
Last Edit: 2023-02-01 22:51:01
Other:
Requires:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

