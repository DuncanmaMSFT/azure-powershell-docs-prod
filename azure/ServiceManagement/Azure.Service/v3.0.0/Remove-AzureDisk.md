---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: d8da56df-3618-41d9-8d28-b13f4c107dd6
schema: 2.0.0
ms.assetid: C10C104D-CC5F-49D3-8169-971BABE36D04
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Remove-AzureDisk.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Remove-AzureDisk.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureDisk

## SYNOPSIS
Removes a disk from the Azure disk repository.

## SYNTAX

```
Remove-AzureDisk [-DiskName] <String> [-DeleteVHD] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureDisk** cmdlet removes a disk from the Azure disk repository in the current subscription.
By default, this cmdlet does not delete the virtual hard disk (VHD) file from blob storage.
To delete the VHD, specify the *DeleteVHD* parameter.

## EXAMPLES

### Example 1: Remove a disk
```
PS C:\>Remove-AzureDisk -DiskName "ContosoDataDisk"
```

This command removes the disk named ContosoDataDisk disk from the disk repository.
The command does not delete the VHD.

### Example 2: Remove and delete a disk
```
PS C:\>Remove-AzureDisk -DiskName "ContosoDataDisk" -DeleteVHD
```

This command removes the disk named ContosoDataDisk disk from the disk repository.
This command specifies the DeleteVHD parameter.
Therefore, the command deletes the VHD from Azure Storage.

## PARAMETERS

### -DiskName
Specifies the name of the data disk in the disk repository that this cmdlet removes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeleteVHD
Indicates that this cmdlet removes the VHD from blob storage.

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

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureDisk](./Add-AzureDisk.md)

[Get-AzureDisk](./Get-AzureDisk.md)

[Update-AzureDisk](./Update-AzureDisk.md)


