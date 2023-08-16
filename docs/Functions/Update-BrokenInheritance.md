---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Update-BrokenInheritance

## SYNOPSIS
Finds and fixes users with broken inheritance.

## SYNTAX

```
Update-BrokenInheritance [[-SearchBase] <String>] [[-Identity] <String>] [<CommonParameters>]
```

## DESCRIPTION
Will search Active Directory for users that do not have permissions inheritance enabled and then fix the inheritance.

## EXAMPLES

### EXAMPLE 1
```
Update-BrokenInheritance -Identity "CN=Joe Snuffy,CN=Users,DC=wstools,DC=dev"
```

Will fix the broken inheritance on the user Joe Snuffy.

### EXAMPLE 2
```
Update-BrokenInheritance -SearchBase "CN=Users,DC=wstools,DC=dev"
```

Will fix the broken inheritance on all users in the Users OU.

## PARAMETERS

### -Identity
Specify a user to fix the inheritance on.
Can use sAMAccountName or distinguishedName.
If no user is specified it will find all users with broken inheritance.

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

### -SearchBase
Specify the OU to search using the distinguishedName of the OU.
If not specified it searches the whole domain.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: (Get-ADDomain).DistinguishedName
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
## OUTPUTS

### System.String
## NOTES
Author: Skyler Hart
Created: Sometime before 2017-08-07
Last Edit: 2022-09-05 23:40:29
Other:
Requires:
    -Module ActiveDirectory

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

