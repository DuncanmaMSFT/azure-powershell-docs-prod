---
external help file: Microsoft.Azure.Commands.Dns.dll-Help.xml
online version: http://azure.microsoft.com/en-us/documentation/articles/azure-preview-portal-using-tags/
schema: 2.0.0
ms.assetid: 15C1904E-7AF9-4836-9E96-C4F0F156E00F
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v0.9.8/New-AzureDnsZone.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v0.9.8/New-AzureDnsZone.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureDnsZone

## SYNOPSIS
Creates a new DNS zone.

## SYNTAX

```
New-AzureDnsZone -Name <String> -ResourceGroupName <String> [-Tag <Hashtable[]>] [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureDnsZone** cmdlet creates a new Domain Name System (DNS) zone in the specified resource group.
You must specify a unique name for the *Name* parameter or the cmdlet will return an error.
After the zone is created, use the **New-AzureDnsRecordSet** cmdlet to create record sets in the zone.

## EXAMPLES

### Example 1: Create a DNS zone
```
PS C:\>$Zone = New-AzureDnsZone -Name "myzone.com" -ResourceGroupName "MyResourceGroup"
```

This command creates a new DNS zone named myzone.com in the specified resource group, and then stores it in the $Zone variable.

## PARAMETERS

### -Name
Specifies the name of the DNS zone to create.

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

### -Profile
Specifies an Azure profile.

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

### -ResourceGroupName
Specifies the resource group in which to create the zone.

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

### -Tag
Specifies an array of tags to associate with the DNS zone.
Tags are name-value pairs represented as hash tables, for example, @(@{"Name"="dept"; "Value"="shopping"}, @{"Name"="env"; "Value"="production"})

```yaml
Type: Hashtable[]
Parameter Sets: (All)
Aliases: Tags

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### Microsoft.Azure.Commands.Dns.DnsZone
This cmdlet returns an object that represents the new DNS zone.

## NOTES

## RELATED LINKS

[Using tags to organize your Azure resources](http://azure.microsoft.com/en-us/documentation/articles/azure-preview-portal-using-tags/)

[Get-AzureDnsZone](./Get-AzureDnsZone.md)

[New-AzureDnsRecordSet](./New-AzureDnsRecordSet.md)

[Remove-AzureDnsZone](./Remove-AzureDnsZone.md)


