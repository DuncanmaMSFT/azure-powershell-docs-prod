---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureApplicationGatewayIPConfiguration.md
schema: 2.0.0
ms.assetid: 418383FD-E450-4729-9628-19C3E4356A09
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureApplicationGatewayIPConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureApplicationGatewayIPConfiguration.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureApplicationGatewayIPConfiguration

## SYNOPSIS
Removes an IP configuration from an application gateway.

## SYNTAX

```
Remove-AzureApplicationGatewayIPConfiguration -Name <String> -ApplicationGateway <PSApplicationGateway>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureApplicationGatewayIPConfiguration** cmdlet removes an IP configuration from an Azure application gateway.

## EXAMPLES

### Example 1: Remove an IP configuration from an azure_2 application gateway.
```
PS C:\>$AppGw = Get-AzureApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> Remove-AzureApplicationGatewayIPConfiguration -ApplicationGateway $AppGw -Name "Subnet02"
```

The first command gets an application gateway and stores it in the $AppGw variable.

The second command removes the IP configuration named Subnet02 from the application gateway stored in $AppGw.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway from which to remove an IP configuration.

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

### -Name
Specifies the name of the IP configuration to remove.

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

## NOTES

## RELATED LINKS

[Add-AzureApplicationGatewayIPConfiguration](./Add-AzureApplicationGatewayIPConfiguration.md)

[Get-AzureApplicationGatewayIPConfiguration](./Get-AzureApplicationGatewayIPConfiguration.md)

[New-AzureApplicationGatewayIPConfiguration](./New-AzureApplicationGatewayIPConfiguration.md)

[Set-AzureApplicationGatewayIPConfiguration](./Set-AzureApplicationGatewayIPConfiguration.md)


