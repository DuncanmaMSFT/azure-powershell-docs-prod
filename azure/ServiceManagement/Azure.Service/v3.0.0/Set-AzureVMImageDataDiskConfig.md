---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: afcc107f-be72-477d-8363-805c388a0878
schema: 2.0.0
ms.assetid: C918B4D5-15B9-4B6F-AA20-7B2CC4729CD9
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureVMImageDataDiskConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureVMImageDataDiskConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureVMImageDataDiskConfig

## SYNOPSIS
Sets the Data Disk properties on the virtual machine image.

## SYNTAX

### UpdateAzureVMImageParamSet (Default)
```
Set-AzureVMImageDataDiskConfig [-DiskConfig] <VirtualMachineImageDiskConfigSet> [-DataDiskName] <String>
 [-Lun] <Int32> [-HostCaching] <String> [<CommonParameters>]
```

### AddAzureVMImageParamSet
```
Set-AzureVMImageDataDiskConfig [-DiskConfig] <VirtualMachineImageDiskConfigSet> [-Lun] <Int32>
 [-HostCaching] <String> [-MediaLink] <Uri> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureVMImageDataDiskConfig** cmdlet sets the Data Disk properties on the virtual machine image.

## EXAMPLES

### Example 1: Set Data Disk properties on a virtual machine image
```
PS C:\>$Disk = New-AzureDiskConfigSet
PS C:\> $Disk = Set-AzureOSDiskConfig -DiskConfig $Disk -HostCaching ReadWrite
PS C:\> $Disk = Set-AzureDataDiskConfig -DiskConfig $Disk -Name "Test" -HostCaching "ReadWrite" -LUN 0
PS C:\> Update-AzureVMImage -ImageName "Image2" -Label "Test1" -Description "Test1" -DiskConfigSet $Disk;
```

This command sets data disk properties on a virtual machine then updates the virtual machine image.

## PARAMETERS

### -DiskConfig
Specifies the disk configuration object that encapsulates the operating system disk and Data Disk objects.

```yaml
Type: VirtualMachineImageDiskConfigSet
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -DataDiskName
Specifies the name of the data disk that this cmdlet configures.

```yaml
Type: String
Parameter Sets: UpdateAzureVMImageParamSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Lun
Specifies the slot where the data drive is mounted in the virtual machine.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -HostCaching
Specifies the host cache attribute for the operating system disk.

Valid values are:

--ReadOnly
--ReadWrite

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -MediaLink
Specifies the URI of the location where the new virtual hard drive is created when the new data disk is added.

```yaml
Type: Uri
Parameter Sets: AddAzureVMImageParamSet
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.WindowsAzure.Commands.ServiceManagement.Model.VirtualMachineImageDiskConfigSet

## NOTES

## RELATED LINKS

[Remove-AzureVMImageDataDiskConfig](./Remove-AzureVMImageDataDiskConfig.md)


