---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Clear-Space

## SYNOPSIS
Clears harddrive space

## SYNTAX

```
Clear-Space [[-ComputerName] <String[]>] [-InvokeMethod] [<CommonParameters>]
```

## DESCRIPTION
Clears harddrive space by clearing temp files and caches.
Invoke method does not clear as many locations. 
#DevSkim: ignore DS104456

## EXAMPLES

### EXAMPLE 1
```
Clear-Space
```

Clears temp and cache data on the local computer

### EXAMPLE 2
```
Clear-Space -ComputerName COMP1
```

Clears temp and cache data on the computer COMP1

### EXAMPLE 3
```
Clear-Space -ComputerName (gc c:\complist.txt)
```

Clears temp and cache data on the computers listed in the file c:\complist.txt

### EXAMPLE 4
```
Clear-Space -ComputerName (gc c:\complist.txt) -InvokeMethod
```

Clears temp and cache data on the computers listed in the file c:\complist.txt using the Invoke-WMIMethod
command. 
#DevSkim: ignore DS104456

## PARAMETERS

### -ComputerName
Specifies the computer or computers to clear space on

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

### -InvokeMethod
Specifies the computer or computers to clear space on using the Invoke-WMIMethod command                        #DevSkim: ignore DS104456

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
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
CREATED: 05/19/2017 20:16:47
LASTEDIT: 07/22/2019 14:21:15
KEYWORDS: Delete, temp, patches, cache, prefetch, SCCM
REMARKS: Needs to be ran as a user that has administrator rights

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

