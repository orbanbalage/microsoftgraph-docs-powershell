---
external help file: Microsoft.Graph.Bookings-help.xml
Module Name: Microsoft.Graph.Bookings
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.bookings/stop-mgbookingbusinessappointment
schema: 2.0.0
---

# Stop-MgBookingBusinessAppointment

## SYNOPSIS
Cancels the giving booking appointment, sending a message to the involved parties.

## SYNTAX

### CancelExpanded1 (Default)
```
Stop-MgBookingBusinessAppointment -BookingAppointmentId <String> -BookingBusinessId <String>
 [-AdditionalProperties <Hashtable>] [-CancellationMessage <String>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Cancel1
```
Stop-MgBookingBusinessAppointment -BookingAppointmentId <String> -BookingBusinessId <String>
 -BodyParameter <IPaths17354LzSolutionsBookingbusinessesBookingbusinessIdAppointmentsBookingappointmentIdMicrosoftGraphCancelPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CancelViaIdentityExpanded1
```
Stop-MgBookingBusinessAppointment -InputObject <IBookingsIdentity> [-AdditionalProperties <Hashtable>]
 [-CancellationMessage <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CancelViaIdentity1
```
Stop-MgBookingBusinessAppointment -InputObject <IBookingsIdentity>
 -BodyParameter <IPaths17354LzSolutionsBookingbusinessesBookingbusinessIdAppointmentsBookingappointmentIdMicrosoftGraphCancelPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Cancels the giving booking appointment, sending a message to the involved parties.

## EXAMPLES

### Example 1: Using the Stop-MgBookingBusinessAppointment Cmdlet
```powershell
Import-Module Microsoft.Graph.Bookings
$params = @{
	CancellationMessage = "Your appointment has been successfully cancelled. Please call us again."
}
Stop-MgBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId -BodyParameter $params
```

This example shows how to use the Stop-MgBookingBusinessAppointment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CancelExpanded1, CancelViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths17354LzSolutionsBookingbusinessesBookingbusinessIdAppointmentsBookingappointmentIdMicrosoftGraphCancelPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Cancel1, CancelViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BookingAppointmentId
The unique identifier of bookingAppointment

```yaml
Type: String
Parameter Sets: CancelExpanded1, Cancel1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BookingBusinessId
The unique identifier of bookingBusiness

```yaml
Type: String
Parameter Sets: CancelExpanded1, Cancel1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CancellationMessage
.

```yaml
Type: String
Parameter Sets: CancelExpanded1, CancelViaIdentityExpanded1
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
Type: IBookingsIdentity
Parameter Sets: CancelViaIdentityExpanded1, CancelViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
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

### Microsoft.Graph.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths17354LzSolutionsBookingbusinessesBookingbusinessIdAppointmentsBookingappointmentIdMicrosoftGraphCancelPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths17354LzSolutionsBookingbusinessesBookingbusinessIdAppointmentsBookingappointmentIdMicrosoftGraphCancelPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CancellationMessage <String>]`: 

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[BookingAppointmentId <String>]`: The unique identifier of bookingAppointment
  - `[BookingBusinessId <String>]`: The unique identifier of bookingBusiness
  - `[BookingCurrencyId <String>]`: The unique identifier of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: The unique identifier of bookingCustomQuestion
  - `[BookingCustomerBaseId <String>]`: The unique identifier of bookingCustomerBase
  - `[BookingCustomerId <String>]`: The unique identifier of bookingCustomer
  - `[BookingServiceId <String>]`: The unique identifier of bookingService
  - `[BookingStaffMemberBaseId <String>]`: The unique identifier of bookingStaffMemberBase
  - `[BookingStaffMemberId <String>]`: The unique identifier of bookingStaffMember
  - `[BusinessScenarioId <String>]`: The unique identifier of businessScenario
  - `[BusinessScenarioTaskId <String>]`: The unique identifier of businessScenarioTask
  - `[PlannerPlanConfigurationLocalizationId <String>]`: The unique identifier of plannerPlanConfigurationLocalization

## RELATED LINKS
