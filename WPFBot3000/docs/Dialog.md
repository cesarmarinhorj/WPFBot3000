---
external help file: WPFBot3000-help.xml
Module Name: wpfbot3000
online version: https://msdn.microsoft.com/en-us/library/system.windows.controls.datepicker
schema: 2.0.0
---

# Dialog

## SYNOPSIS
Creates a window with the requested controls, OK, and Cancel and outputs an object representing the values in the window.

## SYNTAX

```
Dialog [[-Contents] <ScriptBlock>] [[-labelMap] <Hashtable>] [[-Events] <Hashtable[]>] [[-Title] <String>]
 [[-Property] <Hashtable>] [-ShowGridLines] [<CommonParameters>]
```

## DESCRIPTION
Creates a window with the requested controls, OK, and Cancel and outputs an object representing the values in the window.

## EXAMPLES

### EXAMPLE 1
```
Dialog {
```

TextBox FirstName
    TextBox LastName
    TextBox EmailAddress
    DatePicker ReminderDate
} -Title Dialog

# Displays a window with 3 textboxes and a date picker and if the user presses ok (instead of cancel) it outputs an object with 4 properties (populated from the controls)

## PARAMETERS

### -Contents
Scriptblock containing statements that output controls that you want in the dialog.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -labelMap
A hashtable with items of the form ControlName='Desired label'. 
If the control is labeled it will use this text instead of the control name.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: @{}
Accept pipeline input: False
Accept wildcard characters: False
```

### -Events
An array of hashtables of event handlers for controls in the dialog. 
Each should have Name (control name), EventName, and Action.

```yaml
Type: Hashtable[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
The window title

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
A hashtable of properties to set on the window

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowGridLines
Switch to say whether to show grid lines in all grids (for layout debugging)

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
