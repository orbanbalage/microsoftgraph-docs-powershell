---
external help file: Microsoft.Graph.Calendar-help.xml
Module Name: Microsoft.Graph.Calendar
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.calendar/new-mgusereventattachment
schema: 2.0.0
---

# New-MgUserEventAttachment

## SYNOPSIS
Create new navigation property to attachments for users

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserEventAttachment -EventId <String> -UserId <String> [-AdditionalProperties <Hashtable>]
 [-ContentType <String>] [-Id <String>] [-IsInline] [-LastModifiedDateTime <DateTime>] [-Name <String>]
 [-Size <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserEventAttachment -EventId <String> -UserId <String> -BodyParameter <IMicrosoftGraphAttachment>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserEventAttachment -InputObject <ICalendarIdentity> [-AdditionalProperties <Hashtable>]
 [-ContentType <String>] [-Id <String>] [-IsInline] [-LastModifiedDateTime <DateTime>] [-Name <String>]
 [-Size <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserEventAttachment -InputObject <ICalendarIdentity> -BodyParameter <IMicrosoftGraphAttachment> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to attachments for users

## EXAMPLES

### Example 1: Using the New-MgUserEventAttachment Cmdlet
```powershell
Import-Module Microsoft.Graph.Calendar
$params = @{
	"@odata.type" = "#microsoft.graph.fileAttachment"
	Name = "menu.txt"
	ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params
```

This example shows how to use the New-MgUserEventAttachment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 2: Using the New-MgUserEventAttachment Cmdlet
```powershell
Import-Module Microsoft.Graph.Calendar
$params = @{
	"@odata.type" = "#microsoft.graph.itemAttachment"
	Name = "Holiday event"
	Item = @{
		"@odata.type" = "microsoft.graph.event"
		Subject = "Discuss gifts for children"
	}
}
# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params
```

This example shows how to use the New-MgUserEventAttachment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 3: Using the New-MgUserEventAttachment Cmdlet
```powershell
Import-Module Microsoft.Graph.Calendar
$params = @{
	"@odata.type" = "#Microsoft.OutlookServices.ItemAttachment"
	Name = "name-value"
	Item = @{
		"@odata.type" = "microsoft.graph.message"
	}
}
# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params
```

This example shows how to use the New-MgUserEventAttachment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 4: Using the New-MgUserEventAttachment Cmdlet
```powershell
Import-Module Microsoft.Graph.Calendar
$params = @{
	"@odata.type" = "#microsoft.graph.referenceAttachment"
	Name = "Personal pictures"
	SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
	ProviderType = "oneDriveConsumer"
	Permission = "Edit"
	IsFolder = "True"
}
# A UPN can also be used as -UserId.
New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params
```

This example shows how to use the New-MgUserEventAttachment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
attachment
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttachment
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ContentType
The MIME type.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventId
The unique identifier of event

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique idenfier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ICalendarIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsInline
true if the attachment is an inline attachment; otherwise, false.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The attachment's file name.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Size
The length of the attachment in bytes.

```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.ICalendarIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAttachment
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAttachment
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphAttachment>`: attachment
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[ContentType <String>]`: The MIME type.
  - `[IsInline <Boolean?>]`: true if the attachment is an inline attachment; otherwise, false.
  - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Name <String>]`: The attachment's file name.
  - `[Size <Int32?>]`: The length of the attachment in bytes.

INPUTOBJECT `<ICalendarIdentity>`: Identity Parameter
  - `[AttachmentId <String>]`: The unique identifier of attachment
  - `[CalendarGroupId <String>]`: The unique identifier of calendarGroup
  - `[CalendarId <String>]`: The unique identifier of calendar
  - `[CalendarPermissionId <String>]`: The unique identifier of calendarPermission
  - `[EventId <String>]`: The unique identifier of event
  - `[EventId1 <String>]`: The unique identifier of event
  - `[EventId2 <String>]`: The unique identifier of event
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[GroupId <String>]`: The unique identifier of group
  - `[MultiValueLegacyExtendedPropertyId <String>]`: The unique identifier of multiValueLegacyExtendedProperty
  - `[PlaceId <String>]`: The unique identifier of place
  - `[SingleValueLegacyExtendedPropertyId <String>]`: The unique identifier of singleValueLegacyExtendedProperty
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS
