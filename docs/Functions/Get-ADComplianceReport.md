---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Get-ADComplianceReport

## SYNOPSIS
Checks attributes on Active Directory objects against a set of compliance rules.

## SYNTAX

```
Get-ADComplianceReport [[-UserSearchBase] <String[]>] [[-UserGroupSearchBase] <String[]>]
 [[-AdminSearchBase] <String[]>] [[-AdminGroupSearchBase] <String[]>] [[-ComputerSearchBase] <String[]>]
 [[-MSASearchBase] <String[]>] [[-OrganizationalSearchBase] <String[]>] [[-ServerSearchBase] <String[]>]
 [[-ServiceAccountSearchBase] <String[]>] [-SaveADReports] [[-ReportFolder] <String>] [-SaveReport]
 [<CommonParameters>]
```

## DESCRIPTION
Checks attributes on Active Directory objects against a set of compliance rules and provides a report.
It also
takes several attributes and makes them human readable.

## EXAMPLES

### EXAMPLE 1
```
Get-ADComplianceReport
```

Example of how to use this cmdlet.
Will default to OUs in config file.

### EXAMPLE 2
```
Get-ADComplianceReport -UserSearchBase 'OU=Example User OU,DC=wstools,DC=dev'
```

Will search the 'OU=Example User OU,DC=wstools,DC=dev' OU for user objects and report on them.

### EXAMPLE 3
```
Get-ADComplianceReport -UserSearchBase 'OU=Example User OU,DC=wstools,DC=dev' -SaveReport
```

Will search the 'OU=Example User OU,DC=wstools,DC=dev' OU for user objects and because the -ReportFolder parameter
is not used to specify a path, it will save the report to C:\Scripts.

## PARAMETERS

### -AdminGroupSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for group objects that have admins.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AdminSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for admin objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Admin, Admins

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ComputerSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for computer objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Computer, Computers

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -MSASearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for Managed Service Account objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: MSA, MSAs, gMSA, sMSA

Required: False
Position: 6
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OrganizationalSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for org boxes or shared account objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Orgs, Organizational, Shared

Required: False
Position: 7
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ReportFolder
Specify where you want to save reports to.
If you do not specify a path and use either the SaveADReports or
SaveReport switches this defaults to C:\Scripts.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SaveADReports
Will save data pulled from Active Directory to reports for each object matching their type to path in
ReportFolder parameter.

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

### -SaveReport
Will save the report in csv format.
If a path isn't specified using the ReportFolder parameter it will save to
C:\Scripts.

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

### -ServerSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for server objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Servers, MemberServer, MemberServers, DomainControllers

Required: False
Position: 8
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceAccountSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for Service Account objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: ServiceAccounts

Required: False
Position: 9
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserGroupSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for group objects that have users.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserSearchBase
Specify the distinguishedName(s) of organizational units (OUs) to search for user objects.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: User, Users

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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
Created: 2019-07-02 13:32:53
Last Edit: 2023-05-06 21:50:15
Requires:
    -Module ActiveDirectory

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

