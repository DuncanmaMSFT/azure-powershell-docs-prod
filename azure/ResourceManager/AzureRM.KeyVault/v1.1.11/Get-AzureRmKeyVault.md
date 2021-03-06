---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=824799
schema: 2.0.0
ms.assetid: 47A69425-D1E8-4C04-AEFA-5A50E9CC5229
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v1.1.11/Get-AzureRmKeyVault.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v1.1.11/Get-AzureRmKeyVault.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmKeyVault

## SYNOPSIS
Gets key vaults.

## SYNTAX

### GetVaultByName
```
Get-AzureRmKeyVault [-VaultName] <String> [[-ResourceGroupName] <String>] [<CommonParameters>]
```

### ListVaultsByResourceGroup
```
Get-AzureRmKeyVault [-ResourceGroupName] <String> [<CommonParameters>]
```

### ListAllVaultsInSubscription
```
Get-AzureRmKeyVault [-Tag <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmKeyVault** cmdlet gets information about the key vaults in a subscription.
You can view all key vaults instances in a subscription, or filter your results by a resource group or a particular key vault.

Note that although specifying the resource group is optional for this cmdlet when you get a single key vault, you should do so for better performance.

## EXAMPLES

### Example 1: Get all key vaults in your current subscription
```
PS C:\>Get-AzureRMKeyVault
```

This command gets all the key vaults in your current subscription.

### Example 2: Get a specific key vault
```
PS C:\>$MyVault = Get-AzureRMKeyVault -VaultName 'Contoso03Vault'
```

This command gets the key vault named Contoso03Vault in your current subscription, and then stores it in the $MyVault variable.
You can inspect the properties of $MyVault to get details about the key vault.

### Example 3: Get key vaults in a resource group
```
PS C:\>Get-AzureRMKeyVault -ResourceGroupName 'ContosoPayRollResourceGroup'
```

This command gets all the key vaults in the resource group named ContosoPayRollResourceGroup.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group associated with the key vault or key vaults being queried.

```yaml
Type: String
Parameter Sets: GetVaultByName
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ListVaultsByResourceGroup
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tag
Specifies the key and value of the specified tag to filter the list of key vaults by hash table.

```yaml
Type: Hashtable
Parameter Sets: ListAllVaultsInSubscription
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of the key vault.

```yaml
Type: String
Parameter Sets: GetVaultByName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmKeyVault](./New-AzureRmKeyVault.md)

[Remove-AzureRmKeyVault](./Remove-AzureRmKeyVault.md)


