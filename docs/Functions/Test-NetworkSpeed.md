---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Test-NetworkSpeed

## SYNOPSIS
Test network file transfer speeds, upload and download.

## SYNTAX

```
Test-NetworkSpeed [[-LocalPath] <String>] [[-RemotePath] <String>] [[-FileSize] <Int64>] [<CommonParameters>]
```

## DESCRIPTION
Will test the file transfer speed of a generated file and provide you with the speed in Mbps (Megabit) and MBps (Megabyte) for uploads and downloads to a SMB file share.

## EXAMPLES

### EXAMPLE 1
```
Test-NetworkSpeed
```

Example of how to use this cmdlet using the configured values in the WSTools config.ps1 file.

### EXAMPLE 2
```
Test-NetworkSpeed -FileSize 500KB
```

Another example of how to use this cmdlet but with the FileSize parameter.
This example will generate 500 Kilobyte files to transfer.

### EXAMPLE 3
```
Test-NetworkSpeed -FileSize 100MB
```

Another example of how to use this cmdlet but with the FileSize parameter.
This example will generate 100 Megabyte files to transfer.

### EXAMPLE 4
```
Test-NetworkSpeed -FileSize 1GB
```

Another example of how to use this cmdlet but with the FileSize parameter.
This example will generate 1 Gigabyte files to transfer.

### EXAMPLE 5
```
Test-NetworkSpeed -LocalPath C:\Transfer
```

Another example of how to use this cmdlet but with the local path parameter.

### EXAMPLE 6
```
Test-NetworkSpeed -LocalPath D:\Temp -RemotePath \\server1.wstools.dev\Transfer
```

Another example of how to use this cmdlet but with the local and remote path parameters.

## PARAMETERS

### -FileSize
Specifies the file size of the file to be generated and transferred.
Enter in the format xxKB, xxMB, or xxGB.

```yaml
Type: Int64
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalPath
Specifies the path to the local folder where a file will be generated and where a file will be copied to.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemotePath
Specifies the path to the remote folder where a file will be generated and where a file will be copied to.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String, System.Int64
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2022-06-24 18:21:40
Last Edit: 2022-06-24 18:21:40

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

