---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: 6f7c6611-5c56-4f1d-ab98-cdd92d88821c
schema: 2.0.0
ms.assetid: 15634C76-6B34-4E2B-9354-86155827F200
updated_at: 10/20/2016 12:12 AM
ms.date: 10/20/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v2.1.0/New-AzureRmApiManagementContext.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/831f900c1a4babea8fcc8817cfbc25252a1aa872/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v2.1.0/New-AzureRmApiManagementContext.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmApiManagementContext

## SYNOPSIS
Creates an instance of PsAzureApiManagementContext.

## SYNTAX

```
New-AzureRmApiManagementContext -ResourceGroupName <String> -ServiceName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmApiManagementContext** cmdlet creates an instance of **PsAzureApiManagementContext**.
The context is used for all of the API Management service cmdlets.

## EXAMPLES

### Example 1: Create a PsApiManagementContext instance
```
PS C:\>$ApiMgmtContext = New-AzureRmApiManagementContext -ResourceGroupName "ContosoResources" -ServiceName "Contoso"
```

This command creates an instance of **PsApiManagementContext**.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group under which an API Management service is deployed.

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

### -ServiceName
Specifies the name of the deployed API Management service.

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

## OUTPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsAzureApiManagementContext

## NOTES

## RELATED LINKS


