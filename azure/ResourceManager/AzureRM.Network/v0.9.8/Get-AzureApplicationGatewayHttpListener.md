---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureApplicationGatewayHttpListener.md
schema: 2.0.0
ms.assetid: B356F3A9-458A-4D45-AFA3-9C1061B207C6
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Get-AzureApplicationGatewayHttpListener.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Get-AzureApplicationGatewayHttpListener.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureApplicationGatewayHttpListener

## SYNOPSIS
Gets the HTTP listener of an application gateway.

## SYNTAX

```
Get-AzureApplicationGatewayHttpListener [-Name <String>] -ApplicationGateway <PSApplicationGateway>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureApplicationGatewayHttpListener** cmdlet gets the HTTP listener of an application gateway.

## EXAMPLES

### Example 1: Get a specific HTTP listener
```
PS C:\>$Appgw = Get-AzureApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Listener = Get-AzureApplicationGatewayHttpListener -Name "Listener01" -ApplicationGateway $Appgw
```

This command gets an HTTP listener named Listener01.

### Example 2: Get a list of HTTP listeners
```
PS C:\>$Appgw = Get-AzureApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Listeners = Get-AzureApplicationGatewayHttpListener -ApplicationGateway $Appgw
```

This command gets a list of HTTP listeners.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway object that contains the HTTP listener.

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
Specifies the name of the HTTP listener which this cmdlet gets.

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

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayHttpListener

### IEnumerable<Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayHttpListener>

## NOTES

## RELATED LINKS

[Add-AzureApplicationGatewayHttpListener](./Add-AzureApplicationGatewayHttpListener.md)

[New-AzureApplicationGatewayHttpListener](./New-AzureApplicationGatewayHttpListener.md)

[Remove-AzureApplicationGatewayHttpListener](./Remove-AzureApplicationGatewayHttpListener.md)

[Set-AzureApplicationGatewayHttpListener](./Set-AzureApplicationGatewayHttpListener.md)


