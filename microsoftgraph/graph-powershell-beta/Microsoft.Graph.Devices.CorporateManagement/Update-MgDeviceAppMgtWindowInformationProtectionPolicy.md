---
external help file: Microsoft.Graph.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Devices.CorporateManagement
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmgtwindowinformationprotectionpolicy
schema: 2.0.0
---

# Update-MgDeviceAppMgtWindowInformationProtectionPolicy

## SYNOPSIS
Update the navigation property windowsInformationProtectionPolicies in deviceAppManagement

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceAppMgtWindowInformationProtectionPolicy -WindowsInformationProtectionPolicyId <String>
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment1[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-DaysWithoutContactBeforeUnenroll <Int32>] [-Description <String>] [-DisplayName <String>]
 [-EnforcementLevel <WindowsInformationProtectionEnforcementLevel>] [-EnterpriseDomain <String>]
 [-EnterpriseIPRanges <IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]>]
 [-EnterpriseIPRangesAreAuthoritative]
 [-EnterpriseInternalProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseNetworkDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProtectedDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxiedDomains <IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]>]
 [-EnterpriseProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxyServersAreAuthoritative]
 [-ExemptAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ExemptApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-IconsVisible] [-Id <String>]
 [-IndexingEncryptedStoresOrItemsBlocked] [-IsAssigned] [-LastModifiedDateTime <DateTime>]
 [-MdmEnrollmentUrl <String>] [-MinutesOfInactivityBeforeDeviceLock <Int32>]
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-NumberOfPastPinsRemembered <Int32>] [-PasswordMaximumAttemptCount <Int32>] [-PinExpirationDays <Int32>]
 [-PinLowercaseLetters <WindowsInformationProtectionPinCharacterRequirements>] [-PinMinimumLength <Int32>]
 [-PinSpecialCharacters <WindowsInformationProtectionPinCharacterRequirements>]
 [-PinUppercaseLetters <WindowsInformationProtectionPinCharacterRequirements>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnMdmHandoffDisabled] [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-RoleScopeTagIds <String[]>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-WindowsHelloForBusinessBlocked] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceAppMgtWindowInformationProtectionPolicy -WindowsInformationProtectionPolicyId <String>
 -BodyParameter <IMicrosoftGraphWindowsInformationProtectionPolicy1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceAppMgtWindowInformationProtectionPolicy -InputObject <IDevicesCorporateManagementIdentity>
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment1[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-DaysWithoutContactBeforeUnenroll <Int32>] [-Description <String>] [-DisplayName <String>]
 [-EnforcementLevel <WindowsInformationProtectionEnforcementLevel>] [-EnterpriseDomain <String>]
 [-EnterpriseIPRanges <IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]>]
 [-EnterpriseIPRangesAreAuthoritative]
 [-EnterpriseInternalProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseNetworkDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProtectedDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxiedDomains <IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]>]
 [-EnterpriseProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxyServersAreAuthoritative]
 [-ExemptAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ExemptApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-IconsVisible] [-Id <String>]
 [-IndexingEncryptedStoresOrItemsBlocked] [-IsAssigned] [-LastModifiedDateTime <DateTime>]
 [-MdmEnrollmentUrl <String>] [-MinutesOfInactivityBeforeDeviceLock <Int32>]
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-NumberOfPastPinsRemembered <Int32>] [-PasswordMaximumAttemptCount <Int32>] [-PinExpirationDays <Int32>]
 [-PinLowercaseLetters <WindowsInformationProtectionPinCharacterRequirements>] [-PinMinimumLength <Int32>]
 [-PinSpecialCharacters <WindowsInformationProtectionPinCharacterRequirements>]
 [-PinUppercaseLetters <WindowsInformationProtectionPinCharacterRequirements>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnMdmHandoffDisabled] [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-RoleScopeTagIds <String[]>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-WindowsHelloForBusinessBlocked] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceAppMgtWindowInformationProtectionPolicy -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IMicrosoftGraphWindowsInformationProtectionPolicy1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property windowsInformationProtectionPolicies in deviceAppManagement

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Assignments
Navigation property to list of security groups targeted for policy.
To construct, please use Get-Help -Online and see NOTES section for ASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTargetedManagedAppPolicyAssignment1[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AzureRightsManagementServicesAllowed
Specifies whether to allow Azure RMS encryption for WIP

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Policy for Windows information protection without MDM
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionPolicy1
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedDateTime
The date and time the policy was created.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataRecoveryCertificate
Windows Information Protection DataRecoveryCertificate
To construct, please use Get-Help -Online and see NOTES section for DATARECOVERYCERTIFICATE properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DaysWithoutContactBeforeUnenroll
Offline interval before app data is wiped (days)

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The policy's description.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Policy display name.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnforcementLevel
Possible values for WIP Protection enforcement levels

```yaml
Type: WindowsInformationProtectionEnforcementLevel
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseDomain
Primary enterprise domain

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseInternalProxyServers
This is the comma-separated list of internal proxy servers.
For example, '157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59'.
These proxies have been configured by the admin to connect to specific resources on the Internet.
They are considered to be enterprise network locations.
The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISEINTERNALPROXYSERVERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseIPRanges
Sets the enterprise IP ranges that define the computers in the enterprise network.
Data that comes from those computers will be considered part of the enterprise and protected.
These locations will be considered a safe destination for enterprise data to be shared to
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISEIPRANGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseIPRangesAreAuthoritative
Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.
Default is false

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseNetworkDomainNames
This is the list of domains that comprise the boundaries of the enterprise.
Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISENETWORKDOMAINNAMES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProtectedDomainNames
List of enterprise domains to be protected
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISEPROTECTEDDOMAINNAMES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxiedDomains
Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.
Connections to these resources are considered enterprise data.
If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).
A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISEPROXIEDDOMAINS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxyServers
This is a list of proxy servers.
Any server not on this list is considered non-enterprise
To construct, please use Get-Help -Online and see NOTES section for ENTERPRISEPROXYSERVERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxyServersAreAuthoritative
Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.
Default is false

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExemptAppLockerFiles
Another way to input exempt apps through xml files
To construct, please use Get-Help -Online and see NOTES section for EXEMPTAPPLOCKERFILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExemptApps
Exempt applications can also access enterprise data, but the data handled by those applications are not protected.
This is because some critical enterprise applications may have compatibility problems with encrypted data.
To construct, please use Get-Help -Online and see NOTES section for EXEMPTAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionApp[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IconsVisible
Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.
Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique idenfier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IndexingEncryptedStoresOrItemsBlocked
This switch is for the Windows Search Indexer, to allow or disallow indexing of items

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesCorporateManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsAssigned
Indicates if the policy is deployed to any inclusion groups or not.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Last time the policy was modified.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MdmEnrollmentUrl
Enrollment url for the MDM

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MinutesOfInactivityBeforeDeviceLock
Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.
Range is an integer X where 0 \<= X \<= 999.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NeutralDomainResources
List of domain names that can used for work or personal resource
To construct, please use Get-Help -Online and see NOTES section for NEUTRALDOMAINRESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NumberOfPastPinsRemembered
Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.
The largest number you can configure for this policy setting is 50.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then storage of previous PINs is not required.
This node was added in Windows 10, version 1511.
Default is 0.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PasswordMaximumAttemptCount
The number of authentication failures allowed before the device will be wiped.
A value of 0 disables device wipe functionality.
Range is an integer X where 4 \<= X \<= 16 for desktop and 0 \<= X \<= 999 for mobile devices.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinExpirationDays
Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.
The largest number you can configure for this policy setting is 730.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then the user's PIN will never expire.
This node was added in Windows 10, version 1511.
Default is 0.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinLowercaseLetters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinMinimumLength
Integer value that sets the minimum number of characters required for the PIN.
Default value is 4.
The lowest number you can configure for this policy setting is 4.
The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinSpecialCharacters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinUppercaseLetters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectedAppLockerFiles
Another way to input protected apps through xml files
To construct, please use Get-Help -Online and see NOTES section for PROTECTEDAPPLOCKERFILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectedApps
Protected applications can access enterprise data and the data handled by those applications are protected with encryption
To construct, please use Get-Help -Online and see NOTES section for PROTECTEDAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionApp[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectionUnderLockConfigRequired
Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RevokeOnMdmHandoffDisabled
New property in RS2, pending documentation

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RevokeOnUnenrollDisabled
This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.
If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.
If the keys are not revoked, there will be no revoked file cleanup subsequently.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RightsManagementServicesTemplateId
TemplateID GUID to use for RMS encryption.
The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleScopeTagIds
List of Scope Tags for this Entity instance.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SmbAutoEncryptedFileExtensions
Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary
To construct, please use Get-Help -Online and see NOTES section for SMBAUTOENCRYPTEDFILEEXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Version
Version of the entity.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowsHelloForBusinessBlocked
Boolean value that sets Windows Hello for Business as a method for signing into Windows.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowsInformationProtectionPolicyId
The unique identifier of windowsInformationProtectionPolicy

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
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

### Microsoft.Graph.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphWindowsInformationProtectionPolicy1
## OUTPUTS

### System.Boolean
## NOTES
Please use Get-Help -Online.

## RELATED LINKS

[https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmgtwindowinformationprotectionpolicy](https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmgtwindowinformationprotectionpolicy)

