---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\New-AzureApplicationGatewaySku.md
schema: 2.0.0
ms.assetid: 53D9D100-F971-49EF-84A7-061B3DFA9A56
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Get-AzureApplicationGatewaySku.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Get-AzureApplicationGatewaySku.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureApplicationGatewaySku

## SYNOPSIS
Gets the SKU of an application gateway.

## SYNTAX

```
Get-AzureApplicationGatewaySku -ApplicationGateway <PSApplicationGateway> [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureApplicationGatewaySku** cmdlet gets the stock keeping unit (SKU) of an application gateway.

## EXAMPLES

### Example 1: Get an application gateway SKU
```
PS C:\>$AppGW = Get-AzureApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $SKU = Get-AzureApplicationGatewaySku -ApplicationGateway $AppGW
```

This command gets the SKU of an application gateway named ApplicationGateway01.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway object.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureProfile
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

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewaySku

## NOTES

## RELATED LINKS

[New-AzureApplicationGatewaySku](./New-AzureApplicationGatewaySku.md)

[Set-AzureApplicationGatewaySku](./Set-AzureApplicationGatewaySku.md)


