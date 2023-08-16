---
external help file: WSTools-help.xml
Module Name: WSTools
online version: https://wanderingstag.github.io
schema: 2.0.0
---

# Start-CommandMultiThreaded

## SYNOPSIS
Takes a single command and multithreads it.

## SYNTAX

```
Start-CommandMultiThreaded [[-Command] <String>] [[-Objects] <String[]>] [[-MaxThreads] <Int32>]
 [[-MaxTime] <Int32>] [[-SleepTimer] <Int32>] [[-AddParameter] <Hashtable>] [[-AddSwitch] <Array>]
 [<CommonParameters>]
```

## DESCRIPTION
Will multithread any command/cmdlet/function you specify.

## EXAMPLES

### EXAMPLE 1
```
Start-CommandMultiThreaded Clear-Space (gc c:\Scripts\comps.txt)
```

Will run the Clear-Space command against nine of the computers in the comps.txt file at a time.
This is because the -MaxThreads parameter isn't set so it runs at the default of 9 objects at a time.

### EXAMPLE 2
```
gc c:\Scripts\comps.txt | Start-CommandMultiThreaded Clear-Space
```

Will run the Clear-Space command against nine of the computers in the comps.txt file at a time.
This is because the -MaxThreads parameter isn't set so it runs at the default of 9 objects at a time.

### EXAMPLE 3
```
Start-CommandMultiThreaded -Command Get-Service -Objects (gc c:\Scripts\comps.txt) -AddParameter @{"Name" = "wuauserv"} -AddSwitch @('RequiredServices','DependentServices')
```

Will get the service "wuauserv" and it's dependent/required services from the computers listed in comps.txt.

### EXAMPLE 4
```
Start-CommandMultiThreaded -Command Set-AxwayConfig -Objects COMP1,COMP2 -AddParameter @{"ConfigFile" = "C:\PKI\MyOrgsAxwayConfig.txt"}
```

Will set the Axway config file on both the computer COMP1 and COMP2 at the same time using C:\PKI\MyOrgsAxwayConfig.txt on those computers as the file to import.

## PARAMETERS

### -AddParameter
Allows specifying additional parameters beyond what is used in Objects.
Need to format in a hash table.
Ex:
@{"ParameterName" = "Value"}
or
@{"ParameterName" = "Value";"AnotherParameter" = "AnotherValue"}

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddSwitch
Allows specifying additional switches to add to the command you run.
Need to format in a single string or an array of strings.
Ex:
"TotalCount"
or
@("TotalCount","All")

```yaml
Type: Array
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Command
Where you specify the command you want to multithread.

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

### -MaxThreads
The maximum threads to run.
Can cause resource issues.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 9
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxTime
The amount of seconds to run the script after last job (object) is started.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 300
Accept pipeline input: False
Accept wildcard characters: False
```

### -Objects
The arguments that are provided to the command.
Generally used for specifying the name of one or more computers.
However, it can be used for specifying other arguments such as a list of users.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -SleepTimer
The amount of milliseconds between each time the script checks the status of jobs.
For high resource utilization on the system or if the script is going to take longer to run, this should be increased.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 500
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSObject.System.String
## OUTPUTS

### System.Management.Automation.PSCustomObject
## NOTES
Author: Skyler Hart
Created: Sometime before 2017-08-07
Last Edit: 2022-09-05 22:19:49
Other:

## RELATED LINKS

[https://wanderingstag.github.io](https://wanderingstag.github.io)

