---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureRouteConfig.md
schema: 2.0.0
ms.assetid: 593BD334-7229-4D2F-9E21-E188EF064831
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureRouteConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureRouteConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRouteConfig

## SYNOPSIS
Removes a route from a route table.

## SYNTAX

```
Remove-AzureRouteConfig -Name <String> -RouteTable <PSRouteTable> [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRouteConfig** cmdlet removes a route from an Azure route table.

## EXAMPLES

### Example 1: Remove a route
```
PS C:\>Get-AzureRouteTable -ResourceGroupName "ResourceGroup11" -Name "routetable01" | Remove-AzureRouteConfig -Name "route02" | Set-AzureRouteTable
Name              : routetable01
ResourceGroupName : ResourceGroup11
Location          : eastus
Id                : /subscriptions/xxxx-xxxx-xxxx-xxxx/resourceGroups/ResourceGroup11/providers/Microsoft.Networ
                    k/routeTables/routetable01
Etag              : W/"47099b62-60ec-4bc1-b87b-fad56cb8bed1"
ProvisioningState : Succeeded
Tags              : 
Routes            : [
                      {
                        "Name": "route07",
                        "Etag": "W/\"47099b62-60ec-4bc1-b87b-fad56cb8bed1\"",
                        "Id": "/subscriptions/xxxx-xxxx-xxxx-xxxx/resourceGroups/ResourceGroup11/providers/Micro
                    soft.Network/routeTables/routetable01/routes/route07",
                        "AddressPrefix": "10.1.0.0/16",
                        "NextHopType": "VnetLocal",
                        "NextHopIpAddress": null, 
                        "ProvisioningState": "Succeeded"
                      }
                    ] 
Subnets           : []
```

This command gets the route table named routetable01 by using the Get-AzureRouteTable cmdlet.
The command passes that table to the current cmdlet by using the pipeline operator.

The current cmdlet remove the route named route02, and the passes the result to the Set-AzureRouteTable cmdlet, which updates the table to reflect your changes.
The table no longer contains the route named route02.

## PARAMETERS

### -Name
Specifies the name of the route that this cmdlet removes.

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

### -RouteTable
Specifies the route table that contains the route that this cmdlet deletes.

```yaml
Type: PSRouteTable
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRouteConfig](./Add-AzureRouteConfig.md)

[Get-AzureRouteConfig](./Get-AzureRouteConfig.md)

[New-AzureRouteConfig](./New-AzureRouteConfig.md)

[Set-AzureRouteConfig](./Set-AzureRouteConfig.md)


