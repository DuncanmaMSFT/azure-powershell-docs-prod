---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: .\New-AzureRmApiManagementLogger.md
schema: 2.0.0
ms.assetid: A935ABAC-6C60-4AE3-9434-B9BCC1182A34
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.1.4/Get-AzureRmApiManagementLogger.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.1.4/Get-AzureRmApiManagementLogger.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmApiManagementLogger

## SYNOPSIS
Gets API Management Logger objects.

## SYNTAX

### Get all loggers (Default)
```
Get-AzureRmApiManagementLogger -Context <PsApiManagementContext> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Get by logger ID
```
Get-AzureRmApiManagementLogger -Context <PsApiManagementContext> [-LoggerId <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApiManagementLogger** cmdlet gets an azure_2 API Management **Logger** or all the loggers.

## EXAMPLES

### Example 1: Get all loggers
```
PS C:\>Get-AzureRmApiManagementLogger -Context $ApimContext
```

This command gets all the loggers for the specified context.

### Example 2: Get a specific logger
```
PS C:\>Get-AzureRmApiManagementLogger -Context $ApimContext -LoggerId "Logger123"
```

This command removes a logger that has the ID Logger123.

## PARAMETERS

### -Context
Specifies a **PsApiManagementContext** object.

```yaml
Type: PsApiManagementContext
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

### -LoggerId
Specifies the ID of the specific logger to get.

```yaml
Type: String
Parameter Sets: Get by logger ID
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementLogger>

## NOTES

## RELATED LINKS

[New-AzureRmApiManagementLogger](./New-AzureRmApiManagementLogger.md)

[Remove-AzureRmApiManagementLogger](./Remove-AzureRmApiManagementLogger.md)

[Set-AzureRmApiManagementLogger](./Set-AzureRmApiManagementLogger.md)


