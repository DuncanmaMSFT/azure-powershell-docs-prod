---
external help file: Microsoft.Azure.Commands.ManagedCache.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 5DCE8DA4-BD6B-4D99-A89B-32A12563A41E
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v1.6.1/New-AzureManagedCacheNamedCache.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v1.6.1/New-AzureManagedCacheNamedCache.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureManagedCacheNamedCache

## SYNOPSIS
Creates a named cache in the specified Managed Cache Service instance.

## SYNTAX

```
New-AzureManagedCacheNamedCache -Name <String> -NamedCache <String> [-ExpiryPolicy <String>]
 [-ExpiryTime <Int32>] [-WithNotifications] [-WithHighAvailability] [-WithoutEviction]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureManagedCacheNamedCache** cmdlet creates a named cache in the specified azure_2 Managed Cache Service instance in your account and returns an object that represents the new azure_2 cache.
Named caches are supported in the Standard and Premium cache offerings, and are not supported in the Basic cache offering.

## EXAMPLES

### Example 1: Create a named cache in the Managed Cache Service instance
```
PS C:\>New-AzureManagedCacheNamedCache -Name "ContosoCache" -NamedCache "ContosoNamedCache"
```

This command creates a named cache named ContosoNamedCache in the Managed Cache Service instance named ContosoCache.
It uses default values for all the other parameters.

### Example 2: Create a named cache in the specified Managed Cache Service instance with all parameters specified
```
PS C:\>New-AzureManagedCacheNamedCache -Name "ContosoCache" -NamedCache "ContosoNamedCache" -ExpiryPolicy "Sliding" -ExpiryTime 10 -WithNotifications -WithHighAvailability -WithoutEviction
```

This command creates a named cache named ContosoNamedCache in the Managed Cache Service instance named ContosoCache.
It has Notifications and High Availability enabled and Eviction disabled.

## PARAMETERS

### -Name
Specifies the name of the Managed Cache Service instance in which this cmdlet creates a named cache.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NamedCache
Specifies the name of the named cache that this cmdlet creates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpiryPolicy
Specifies the expiry policy for the named cache.
The default value is Absolute.

psdx_paramvalues

- Absolute
- Sliding
- Never

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpiryTime
Specifies the expiry time of the named cache, in minutes.
The default value is 10.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WithHighAvailability
Indicates that high availability is enabled for the named cache.

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

### -WithNotifications
Indicates that notifications are enabled for the named cache.
Notifcations are supported in the Standard and Premium cache offerings, and are unavailable in the Basic cache offering.

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

### -WithoutEviction
Indicates that eviction is disabled for the named cache.

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

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.Azure.Commands.ManagedCache.Models.PSCacheServiceWithNamedCaches

## NOTES
* Use the Add-AzureAccount or Import-AzurePublishSettingsFile cmdlets to make your azure_2 account available to wps_2 before using this cmdlet. For more information, see How to install and configure Azure PowerShellhttp://azure.microsoft.com/en-us/documentation/articles/install-configure-powershell/.

## RELATED LINKS

[Get-AzureManagedCacheNamedCache](./Get-AzureManagedCacheNamedCache.md)

[Remove-AzureManagedCacheNamedCache](./Remove-AzureManagedCacheNamedCache.md)

[Set-AzureManagedCacheNamedCache](./Set-AzureManagedCacheNamedCache.md)


