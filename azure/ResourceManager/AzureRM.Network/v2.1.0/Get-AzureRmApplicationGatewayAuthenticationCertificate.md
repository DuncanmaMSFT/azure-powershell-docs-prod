---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureRmApplicationGatewayAuthenticationCertificate.md
schema: 2.0.0
ms.assetid: E94C6EB0-75B2-41BD-B07A-93BE084FB7CB
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmApplicationGatewayAuthenticationCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmApplicationGatewayAuthenticationCertificate.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmApplicationGatewayAuthenticationCertificate

## SYNOPSIS
Gets an authentication certificate for an application gateway.

## SYNTAX

```
Get-AzureRmApplicationGatewayAuthenticationCertificate [-Name <String>]
 -ApplicationGateway <PSApplicationGateway> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApplicationGatewayAuthenticationCertificate** cmdlet gets an authentication certificate for an Azure application gateway.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Name
Specifies the name of the authentication certificate that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationGateway
Specifies the name of application gateway for which this cmdlet gets an authentication certificate.

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

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayAuthenticationCertificate

## NOTES
* Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayAuthenticationCertificate](./Add-AzureRmApplicationGatewayAuthenticationCertificate.md)

[New-AzureRmApplicationGatewayAuthenticationCertificate](./New-AzureRmApplicationGatewayAuthenticationCertificate.md)

[Remove-AzureRmApplicationGatewayAuthenticationCertificate](./Remove-AzureRmApplicationGatewayAuthenticationCertificate.md)

[Set-AzureRmApplicationGatewayAuthenticationCertificate](./Set-AzureRmApplicationGatewayAuthenticationCertificate.md)


