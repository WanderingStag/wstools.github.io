---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Split-File

## SYNOPSIS

## SYNTAX

```
Split-File [-Path] <String> [[-DestinationFolder] <String>] [[-PartFileSize] <Int32>] [<CommonParameters>]
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

### -DestinationFolder
Enter the path of where you want the part files placed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: OutputLocation, Output, DestinationPath, Destination

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartFileSize
Enter the size you want the part files to be.
Can be bytes or you can specify a size.
Ex: 100MB

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: Size, Newsize

Required: False
Position: 3
Default value: 10485760
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Enter the path of the file you want to split.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Source, InputLocation, SourceFile

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
AUTHOR: Skyler Hart
CREATED: 04/30/2019 13:18:22
LASTEDIT: 2021-12-17 21:13:05
KEYWORDS:
REQUIRES:
    #Requires -Version 3.0

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

