---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 1f74deb4-e9b0-4aeb-8e13-b1554a4ebbec
schema: 2.0.0
ms.assetid: AAC92C22-37DE-491B-A774-38D10675F5A5
updated_at: 10/24/2016 11:18 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackVNet.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7db57df6b5e709a7c001e6de362a1240d7583ae8/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackVNet.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-WAPackVNet

## SYNOPSIS
Gets virtual networks.

## SYNTAX

### Empty (Default)
```
Get-WAPackVNet [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromId
```
Get-WAPackVNet [-ID] <Guid> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromName
```
Get-WAPackVNet [-Name] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-WAPackVNet** cmdlet gets virtual networks.

## EXAMPLES

### Example 1: Get all virtual networks
```
PS C:\>Get-WAPackVNet
```

This command gets all virtual networks.

### Example 2: Get a virtual network by using an ID
```
PS C:\>Get-WAPackVNet -ID 66242D17-189F-480D-87CF-8E1D749998C8
```

This command gets the virtual network that has the specified ID.

### Example 3: Get a virtual network by using a name
```
PS C:\>Get-WAPackVNet -Name "ContosoVNet08"
```

This command gets the virtual network named ContosoVNet08.

## PARAMETERS

### -ID
Specifies the unique ID of a virtual network.

```yaml
Type: Guid
Parameter Sets: FromId
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of a virtual network.

```yaml
Type: String
Parameter Sets: FromName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
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

## OUTPUTS

## NOTES

## RELATED LINKS


