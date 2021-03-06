---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B1F97A23-700A-4A7E-B8C9-26DF98B25994
updated_at: 10/24/2016 11:18 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackLogicalNetwork.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7db57df6b5e709a7c001e6de362a1240d7583ae8/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackLogicalNetwork.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-WAPackLogicalNetwork

## SYNOPSIS
Gets logical network objects.

## SYNTAX

### Empty (Default)
```
Get-WAPackLogicalNetwork [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromName
```
Get-WAPackLogicalNetwork [[-Name] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see  Azure WAPack Cmdletshttp://msdn.microsoft.com/library/dn776450.aspx.
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type (get-module azure).version.

The **Get-WAPackLogicalNetwork** cmdlet gets logical network objects.

## EXAMPLES

### Example 1: Get a logical network by using a name
```
PS C:\>Get-WAPackLogicalNetwork -Name "ContosoLogicalNetwork01"
```

This command gets a logical network named ContosoLogicalNetwork01.

### Example 2: Get all logical networks
```
PS C:\>Get-WAPackLogicalNetwork
```

This command gets all logical networks.

## PARAMETERS

### -Name
Specifies the name of a logical network.

```yaml
Type: String
Parameter Sets: FromName
Aliases: 

Required: False
Position: 0
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


