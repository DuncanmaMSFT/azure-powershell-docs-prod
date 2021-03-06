---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: .\Get-AzureRmVM.md
schema: 2.0.0
ms.assetid: BB359FEA-F61B-420F-ABED-9AAE37FB2EEA
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Get-AzureRmVMSize.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Get-AzureRmVMSize.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmVMSize

## SYNOPSIS
Gets available virtual machine sizes.

## SYNTAX

### ListVirtualMachineSizeParamSet (Default)
```
Get-AzureRmVMSize [-Location] <String> [<CommonParameters>]
```

### ListAvailableSizesForAvailabilitySet
```
Get-AzureRmVMSize [-ResourceGroupName] <String> [-AvailabilitySetName] <String> [<CommonParameters>]
```

### ListAvailableSizesForVirtualMachine
```
Get-AzureRmVMSize [-ResourceGroupName] <String> [-VMName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmVMSize** cmdlet gets available virtual machine sizes.

## EXAMPLES

### Example 1: Get virtual machine sizes for a location
```
PS C:\>Get-AzureRmVMSize -Location "Central US"
```

This command gets the available sizes for virtual machines in the specified location.

### Example 2: Get sizes for an availability set
```
PS C:\>Get-AzureRmVMSize -ResourceGroupName "ResourceGroup03" -AvailabilitySetName "AvailabilitySet17"
```

This command gets available sizes for virtual machines that you can deploy in the availability set named AvailabilitySet17.

### Example 3: Get sizes for an existing virtual machine
```
PS C:\>Get-AzureRmVMSize -ResourceGroupName "ResourceGroup03" -VMName "VirtualMachine12"
```

This command gets available sizes for the existing virtual machine named VirtualMachine12.
You can resize this virtual machine to the sizes that this command gets.

## PARAMETERS

### -AvailabilitySetName
Specifies the name of the Availability Set for which this cmdlet gets the available virtual machine sizes.

```yaml
Type: String
Parameter Sets: ListAvailableSizesForAvailabilitySet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Specifies the location for which this cmdlet gets the available virtual machine sizes.

```yaml
Type: String
Parameter Sets: ListVirtualMachineSizeParamSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the virtual machine.

```yaml
Type: String
Parameter Sets: ListAvailableSizesForAvailabilitySet, ListAvailableSizesForVirtualMachine
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VMName
Specifies the name of the virtual machine that this cmdlet gets the available virtual machine sizes for resizing.

```yaml
Type: String
Parameter Sets: ListAvailableSizesForVirtualMachine
Aliases: 

Required: True
Position: 2
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

[Get-AzureRmVM](./Get-AzureRmVM.md)


