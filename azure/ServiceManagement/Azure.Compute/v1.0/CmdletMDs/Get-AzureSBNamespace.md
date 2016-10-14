---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.0/CmdletMDs/Get-AzureSBNamespace.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.0/CmdletMDs/Get-AzureSBNamespace.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# Get-AzureSBNamespace

## SYNOPSIS
Gets the namespace.

## SYNTAX

```
Get-AzureSBNamespace [[-Name] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
powershell_prelim

The **Get-AzureSBNamespace** cmdlet returns the Service Bus service namespaces associated with the current subscription.

## EXAMPLES

### 1: Get the Service Bus namespace
```
PS C:\>Get-AzureSBNamespace
```

This example gets the Service Bus service namespaces associated with the current subscription.

## PARAMETERS

### -Name
Specifies the name of a Service Bus namespace to look for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
In-memory profile.```yaml
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

[Get-AzureSBLocation](.\Get-AzureSBLocation.md)
