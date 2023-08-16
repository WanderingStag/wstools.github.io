---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-IPrange

## SYNOPSIS
Lists IPs within a range, subnet, or CIDR block.

## SYNTAX

```
Get-IPrange [[-IP] <String>] [-CIDR <String>] [-Subnet <String>] [-Start <String>] [-End <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Lists IPs within a range, subnet, or CIDR block.

## EXAMPLES

### EXAMPLE 1
```
Get-IPrange -ip 192.168.0.3 -subnet 255.255.255.192
```

Will show all IPs within the 192.168.0.0 space with a subnet mask of 255.255.255.192 (CIDR 26.)

### EXAMPLE 2
```
Get-IPrange -PARAMETER
```

Another example of how to use this cmdlet but with a parameter or switch.

## PARAMETERS

### -CIDR
Specifies what CIDR block notation you want to list IPs from.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Notation, Block

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -End
The ending IP in a range.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IP
An IP from the subnet mask or CIDR block you want a range for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: IPv4, Address, IPv4Address

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Start
Specifies a path to one or more locations.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subnet
The subnet mask you want a range for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Mask

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
Created: Sometime before 8/7/2017
Last Edit: 2020-08-20 09:11:46

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

