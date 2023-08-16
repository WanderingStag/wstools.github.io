---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Set-ChromeDeveloperTools

## SYNOPSIS
Will enable or disable Chrome Developer tools.

## SYNTAX

```
Set-ChromeDeveloperTools [-Disable] [<CommonParameters>]
```

## DESCRIPTION
Sets the registry entry HKLM:\SOFTWARE\Policies\Google\Chrome\DeveloperToolsDisabled to 1 (Disabled) or 0 (Enabled)

## EXAMPLES

### EXAMPLE 1
```
Set-ChromeDeveloperTools
```

Example of how to use this cmdlet to enable Chrome Developer Tools.

### EXAMPLE 2
```
Set-ChromeDeveloperTools -Disable
```

Example of how to use this cmdlet to disable Chrome Developer Tools.

## PARAMETERS

### -Disable
Will Disable Chrome Developer Tools.

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

### System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: 2022-09-20 19:53:22
Last Edit: 2022-09-20 19:53:22
Other:
Requires:
    -RunAsAdministrator

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

