---
external help file: WPFBot3000-help.xml
Module Name: wpfbot3000
online version: https://msdn.microsoft.com/en-us/library/system.windows.controls.radiobutton
schema: 2.0.0
---

# RadioButton

## SYNOPSIS
A RadioButton control that encapsulates the Windows Presentation Foundation (WPF) System.Windows.Controls.RadioButton class

## SYNTAX

```
RadioButton [[-Name] <String>] [[-InitialValue] <Boolean>] [[-GroupName] <String>] [[-property] <Hashtable>]
 [<CommonParameters>]
```

## DESCRIPTION
Outputs a RadioButton control. 
Set the initial "checked" state with the -InitialValue parameter, and set any control properties using the -Property parameter.

## EXAMPLES

### EXAMPLE 1
```
Dialog {
```

StackPanel -Name Options -orientation Horizontal {
       RadioButton Eeny -groupName Options
       RadioButton Meeny -InitialValue $true -groupName Options
       RadioButton Miny  -groupName Options
    }
    TextBox Moe
}
\`\`\`
In the window there will be three radio buttons, labeled Eeny, Meeny, and Miny.

## PARAMETERS

### -Name
The name of the control. 
This will be the name of a property in the output of the Dialog function.

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

### -InitialValue
True means checked, False means not checked

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupName
The group that the radio button belongs to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -property
Properties to extend/override the base properties defined in the function

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: @{}
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[https://msdn.microsoft.com/en-us/library/system.windows.controls.radiobutton](https://msdn.microsoft.com/en-us/library/system.windows.controls.radiobutton)

