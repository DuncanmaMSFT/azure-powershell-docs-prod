---
external help file: Microsoft.Azure.Commands.RedisCache.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 648D7776-5056-4025-8706-3BA091658AD0
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.RedisCache/v1.1.10/Set-AzureRmRedisCacheDiagnostics.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.RedisCache/v1.1.10/Set-AzureRmRedisCacheDiagnostics.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmRedisCacheDiagnostics

## SYNOPSIS
Enables diagnostics on an azure_2 Redis Cache.

## SYNTAX

```
Set-AzureRmRedisCacheDiagnostics -ResourceGroupName <String> -Name <String> -StorageAccountId <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmRedisCacheDiagnostics** cmdlet enables diagnostics for an azure_2 Redis Cache.

## EXAMPLES

### Example 1: Enable diagnostics
```
PS C:\>Set-AzureRmRedisCacheDiagnostics -ResourceGroupName "ContosoResourceGroup" -Name "PeakCache" -StorageAccountId "/subscriptions/fffff139-aaaa-bbbb-cccc-21f21f35806e/resourcegroups/myresourcegroup/providers/Microsoft.Storage/storageAccounts/mystorageaccount"
```

This command enables diagnostics for an azure_2 Redis cache.

This command will enable diagnostics or update the storage account for all azure_2 Redis Caches in the same region for the subscription.

## PARAMETERS

### -Name
Specifies the name of the cache.

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

### -ResourceGroupName
Specifies the name of the resource group that contains the cache.

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

### -StorageAccountId
Specifies the resource ID of the storage account used to store the diagnostics data.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Void

## NOTES
* Keywords: azure, azurerm, arm, resource, management, manager, redis, cache, web, webapp, website

## RELATED LINKS

[Remove-AzureRmRedisCacheDiagnostics](./Remove-AzureRmRedisCacheDiagnostics.md)


