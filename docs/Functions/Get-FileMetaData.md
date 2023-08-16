---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://devblogs.microsoft.com/scripting/
#Requires -Version 2.0
schema: 2.0.0
---

# Get-FileMetaData

## SYNOPSIS
This function gets file metadata and returns it as a custom PS Object.

## SYNTAX

```
Get-FileMetaData [[-Path] <String[]>]
```

## DESCRIPTION
This function gets file metadata using the Shell.Application object and
returns a custom PSObject object that can be sorted, filtered or otherwise
manipulated.

## EXAMPLES

### EXAMPLE 1
```
Get-FileMetaData -Path "e:\music"
```

Gets file metadata for all files in the e:\music directory

### EXAMPLE 2
```
Get-FileMetaData -Path (gci e:\music -Recurse -Directory).FullName
```

This example uses the Get-ChildItem cmdlet to do a recursive lookup of
all directories in the e:\music folder and then it goes through and gets
all of the file metada for all the files in the directories and in the
subdirectories.

### EXAMPLE 3
```
Get-FileMetaData -Path "c:\fso","E:\music\Big Boi"
```

Gets file metadata from files in both the c:\fso directory and the
e:\music\big boi directory.

### EXAMPLE 4
```
$meta = Get-FileMetaData -Path "E:\music"
```

This example gets file metadata from all files in the root of the
e:\music directory and stores the returned custom objects in a $meta
variable for later processing and manipulation.

## PARAMETERS

### -Path
The path that is parsed for files

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
NAME:  Get-FileMetaData
AUTHOR: ed wilson, msft
Edited By: Skyler Hart
Original: 01/24/2014 14:08:24
Last Edit: 2021-12-19 18:54:58
KEYWORDS: Storage, Files, Metadata

## RELATED LINKS

[https://devblogs.microsoft.com/scripting/
#Requires -Version 2.0](https://devblogs.microsoft.com/scripting/
#Requires -Version 2.0)

