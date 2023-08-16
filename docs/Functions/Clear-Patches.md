---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Clear-Patches

## SYNOPSIS
Clears the C:\Patches folder.

## SYNTAX

```
Clear-Patches [-ObjectList] <String[]> [-Recursive] [-Old] [[-MaxThreads] <Int32>] [[-SleepTimer] <Object>]
 [[-MaxResultTime] <Object>] [<CommonParameters>]
```

## DESCRIPTION
Removes items in the C:\Patches folder on the local or remote computer.

## EXAMPLES

### EXAMPLE 1
```
Clear-Patches
```

Clears C:\Patches folder on the local computer (but not the inidividual program folders.)

### EXAMPLE 2
```
Clear-Patches -ComputerName COMP1
```

Clears C:\Patches folder on the computer COMP1.

### EXAMPLE 3
```
Clear-Patches -ComputerName (gc c:\complist.txt) -Recursive
```

Clears all files and folders in C:\Patches on the computers listed in the file c:\complist.txt.

### EXAMPLE 4
```
Clear-Patches -ComputerName (gc c:\complist.txt) -Old
```

Clears files in the root of C:\Patches that are older than 28 days on the computers listed in the file c:\complist.txt.

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

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Old
Removes files in the root of the C:\Patches folder (except Install.ps1) that are older than 28 days.

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

### -Recursive
Removes all files and folders in the Patches folder on the specified computer.

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
Created: 2020-08-18 09:58:51
Last Edit: 2020-08-18 09:58:51
Keywords: Delete, temp, patches
Other: Needs to be ran as a user that has administrator rights
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

