---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
online version: .\Get-AzureRmBackupVault.md
schema: 2.0.0
ms.assetid: 842FB465-085D-41C6-86BC-9C57549DDE4B
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.1.0/Set-AzureRmBackupVault.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.1.0/Set-AzureRmBackupVault.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmBackupVault

## SYNOPSIS
Changes the storage type of a Backup vault.

## SYNTAX

```
Set-AzureRmBackupVault [[-Storage] <AzureBackupVaultStorageType>] [-Vault] <AzureRMBackupVault>
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmBackupVault** cmdlet changes the storage type of an Azure Backup vault.
You cannot modify other properties of a vault.

## EXAMPLES

### Example 1: Change the storage for an existing vault
```
PS C:\>Get-AzureRmBackupVault -Name "Vault03" | Set-AzureRmBackupVault -Storage LocallyRedundant
```

This command gets the Azure Backup vault named Vault03 by using the **Get-AzureRmBackupVault** cmdlet.
The command passes that vault to the current cmdlet by using the pipeline operator.
The current cmdlet changes the storage type to LocallyRedundant.

## PARAMETERS

### -Storage
Specifies the storage type for the backup data.
The acceptable values for this parameter are: LocallyRedundant and GeoRedundant.

```yaml
Type: AzureBackupVaultStorageType
Parameter Sets: (All)
Aliases: 
Accepted values: GeoRedundant, LocallyRedundant

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Vault
Specifies a Backup vault that this cmdlet modifies.
To obtain an **AzureRmBackupVault** object, use the Get-AzureRmBackupVault cmdlet.

```yaml
Type: AzureRMBackupVault
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### AzureRmBackupVault

## OUTPUTS

### None

## NOTES
* When you register the first server or virtual machine for a vault, the storage type is locked. Subsequently, you cannot change the storage type.

## RELATED LINKS

[Get-AzureRmBackupVault](./Get-AzureRmBackupVault.md)

[New-AzureRmBackupVault](./New-AzureRmBackupVault.md)

[Remove-AzureRmBackupVault](./Remove-AzureRmBackupVault.md)


