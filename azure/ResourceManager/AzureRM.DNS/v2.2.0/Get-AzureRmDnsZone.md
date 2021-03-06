---
external help file: Microsoft.Azure.Commands.Dns.dll-Help.xml
online version: 8cdd0580-1174-4f34-849d-d0f18baff439
schema: 2.0.0
ms.assetid: B5A63F24-76B7-440C-8D5A-6362849AFC20
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v2.2.0/Get-AzureRmDnsZone.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v2.2.0/Get-AzureRmDnsZone.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmDnsZone

## SYNOPSIS
Gets a DNS zone.

## SYNTAX

### Default (Default)
```
Get-AzureRmDnsZone [<CommonParameters>]
```

### ResourceGroup
```
Get-AzureRmDnsZone [-Name <String>] -ResourceGroupName <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmDnsZone** cmdlet gets a Domain Name System (DNS) zone from the specified resource group.
If you specify the *Name* parameter, a single **DnsZone** object is returned.
If you do not specify the *Name* parameter, an array containing all of the zones in the specified resource group is returned.
You can use the **DnsZone** object to update the zone, for example you can add **RecordSet** objects to it.

## EXAMPLES

### Example 1: Get a zone
```
PS C:\> $Zone = Get-AzureRmDnsZone -ResourceGroupName "MyResourceGroup" -Name "myzone.com"
```

This example gets the DNS zone named myzone.com from the specified resource group, and then stores it in the $Zone variable.

### Example 2: Get all of the zones in a resource group
```
PS C:\> $Zones = Get-AzureRmDnsZone -ResourceGroupName "MyResourceGroup"
```

This example gets all of the DNS zones in the specified resource group, and then stores it in the $Zones variable.

### Example 3: Get all of the zones in a subscription
```
PS C:\> $Zones = Get-AzureRmDnsZone
```

This example gets all of the DNS zones in the current azure_2 subscription, and then stores them in the $Zones variable.

## PARAMETERS

### -Name
Specifies the name of the DNS zone to get.

If you do not specify a value for the *Name* parameter, this cmdlet gets all DNS zones in the specified resource group.
If you also omit the *ResourceGroupName* parameter, this cmdlet gets all DNS zones in the current azure_2 subscription.

```yaml
Type: String
Parameter Sets: ResourceGroup
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the DNS zone to get.

If you do not specify the *ResourceGroupName*, then you mus also omit the *Name* parameter.
In this case, this cmdlet gets all DNS zones in the current azure_2 subscription.

```yaml
Type: String
Parameter Sets: ResourceGroup
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
This cmdlet does not allow you to pipe input.

## OUTPUTS

### Microsoft.Azure.Commands.Dns.DnsZone
This cmdlet returns an object that represents the DNS zone.
If the zone name is not specified, an array of zone objects is returned.

## NOTES

## RELATED LINKS

[New-AzureRmDnsZone](./New-AzureRmDnsZone.md)

[Remove-AzureRmDnsZone](./Remove-AzureRmDnsZone.md)

[Set-AzureRmDnsZone](./Set-AzureRmDnsZone.md)


