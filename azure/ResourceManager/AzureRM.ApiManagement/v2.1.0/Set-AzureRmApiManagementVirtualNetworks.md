---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version: .\New-AzureRmApiManagementVirtualNetwork.md
schema: 2.0.0
ms.assetid: C667EF41-1FB3-40C3-884A-8F008520A68C
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v2.1.0/Set-AzureRmApiManagementVirtualNetworks.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v2.1.0/Set-AzureRmApiManagementVirtualNetworks.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmApiManagementVirtualNetworks

## SYNOPSIS
Sets the VPN configuration for an API Management Service.

## SYNTAX

```
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName <String> -Name <String>
 [-VirtualNetworks <PsApiManagementVirtualNetwork[]>] [-PassThru] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmApiManagementVirtualNetworks** cmdlet sets Virtual Network configuration for an API Management service.

## EXAMPLES

### Example 1: Set virtual networks for an API Management service
```
PS C:\>Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $VirtualNetworks
```

This command sets virtual networks for an API Management service.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group under which the API Management service exists.

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

### -Name
Specifies the name of an API Management service.

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

### -VirtualNetworks
Specifies an array of virtual networks configurations.
Passing $null will remove the virtual network configuration.

```yaml
Type: PsApiManagementVirtualNetwork[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

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

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

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

[New-AzureRmApiManagementVirtualNetwork](./New-AzureRmApiManagementVirtualNetwork.md)


