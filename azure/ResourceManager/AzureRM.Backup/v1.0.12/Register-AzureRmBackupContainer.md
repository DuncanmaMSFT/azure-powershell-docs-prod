---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
online version: .\Get-AzureRmBackupVault.md
schema: 2.0.0
ms.assetid: 1800F1EE-FE68-42EB-AB56-A8D464B84793
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v1.0.12/Register-AzureRmBackupContainer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v1.0.12/Register-AzureRmBackupContainer.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Register-AzureRmBackupContainer

## SYNOPSIS
Registers the container with a Backup vault.

## SYNTAX

### V1VM
```
Register-AzureRmBackupContainer -Name <String> -ServiceName <String> [-Vault] <AzureRMBackupVault>
 [<CommonParameters>]
```

### V2VM
```
Register-AzureRmBackupContainer -Name <String> -ResourceGroupName <String> [-Vault] <AzureRMBackupVault>
 [<CommonParameters>]
```

## DESCRIPTION
The **Register-AzureRmBackupContainer** cmdlet registers the container with an azure_2 Backup vault.
To configure backup by using azure_2 Backup, first register your server or virtual machine with a Backup vault.
This cmdlet registers an infrastructure as a service (IaaS) virtual machine with the specified vault.
The register operation associates the azure_2 virtual machine with the backup vault and tracks the virtual machine through the backup life cycle.

## EXAMPLES

### Example 1: Register a virtual machine to a Backup vault
```
PS C:\>$Vault = Get-AzureRmBackupVault -Name "Vault03"
PS C:\> Register-AzureRmBackupContainer -Vault $Vault -Name "Contoso03Vm" -ServiceName "ContosoService27"
```

The first command gets the vault named Vault03 by using the Get-AzureRmBackupVault cmdlet.
The command stores the vault in the $Vault variable.

The second command registers the virtual machine named Contoso03Vm with the vault in $Vault.
That virtual machine belongs to the service named ContosoService27.

## PARAMETERS

### -Name
Specifies the name of the virtual machine that this cmdlet registers.

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
Specifies the name of the resource group for the virtual machine.

```yaml
Type: String
Parameter Sets: V2VM
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Specifies the service name of the virtual machine that this cmdlet registers.

Typically, a cloud service name has a suffix .cloudapp.net.
Do not include the suffix when you specify this parameter.

To obtain information about a virtual machine, use the Get-AzureRMVM cmdlet.
The service name is the **DeploymentName** property of the virtual machine object.

```yaml
Type: String
Parameter Sets: V1VM
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Vault
Specifies the Backup vault to which this cmdlet registers virtual machine.
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

### AzureRmBackupJob

## NOTES

## RELATED LINKS

[Get-AzureRmBackupVault](./Get-AzureRmBackupVault.md)


