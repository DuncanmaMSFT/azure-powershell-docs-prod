---
external help file: Microsoft.Azure.Commands.ManagedCache.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 06F96135-1624-4693-AD49-30B2BE41A19E
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v2.1.0/Remove-AzureManagedCacheNamedCache.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v2.1.0/Remove-AzureManagedCacheNamedCache.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureManagedCacheNamedCache

## SYNOPSIS
Removes a named cache from a Managed Cache Service instance.

## SYNTAX

```
Remove-AzureManagedCacheNamedCache -Name <String> -NamedCache <String> [-Force] [-PassThru]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureManagedCacheNamedCache** cmdlet removes a named cache from the specified Azure Managed Cache Service instance in your Azure account.

## EXAMPLES

### Example 1: Remove the specified named cache from the specified Managed Cache Service instance
```
PS C:\>Remove-AzureManagedCacheNamedCache -Name "ContosoCache" -NamedCache "ContosoNamedCache" -Force -PassThru
```

This command removes an Azure cache named ContosoNamedCache.

## PARAMETERS

### -Name
Specifies the name of the Managed Cache Service instance from which to remove the named cache.

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
Specifies the name of the named cache that this cmdlet removes.

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

### -Force
Forces the command to run without asking for user confirmation.

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

### -PassThru
Indicates that this cmdlet returns a Boolean that indicates the success of the operation.

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
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### Boolean

## NOTES
* Use the Add-AzureAccount or Import-AzurePublishSettingsFile to make your Azure account available to Windows PowerShell before using this cmdlet. For more information, see How to install and configure Azure PowerShellhttp://azure.microsoft.com/en-us/documentation/articles/install-configure-powershell/.

## RELATED LINKS

[How to install and configure Azure PowerShell](http://azure.microsoft.com/en-us/documentation/articles/install-configure-powershell/)

[Get-AzureManagedCacheNamedCache](./Get-AzureManagedCacheNamedCache.md)

[New-AzureManagedCacheNamedCache](./New-AzureManagedCacheNamedCache.md)

[Set-AzureManagedCacheNamedCache](./Set-AzureManagedCacheNamedCache.md)


