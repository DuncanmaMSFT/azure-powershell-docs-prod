---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: .\Export-AzureRmApiManagementApi.md
schema: 2.0.0
ms.assetid: B80389B9-E143-4E24-A222-E95F691DA2E9
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.1.4/Get-AzureRmApiManagementApi.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.1.4/Get-AzureRmApiManagementApi.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmApiManagementApi

## SYNOPSIS
Gets an API.

## SYNTAX

### All APIs (Default)
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Find by ID
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -ApiId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Find by Name
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -Name <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Find by product ID
```
Get-AzureRmApiManagementApi -Context <PsApiManagementContext> -ProductId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApiManagementApi** cmdlet gets one or more azure_2 API Management APIs.

## EXAMPLES

### Example 1: Get all management APIs
```
PS C:\>Get-AzureRmApiManagementApi -Context $ApiMgmtContext
```

This command gets all of the APIs for the specified context.

### Example 2: Get a management API by ID
```
PS C:\>Get-AzureRmApiManagementApi -Context $ApiMgmtContext -ApiId $ApiId
```

This command gets the API with the specified ID.

### Example 3: Get a management API by name
```
PS C:\>Get-AzureRmApiManagementApi -Context $ApiMgmtContext -Name "EchoApi"
```

This command gets the API with the specified name.

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

### -ApiId
Specifies the ID of the API to get.

```yaml
Type: String
Parameter Sets: Find by ID
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the API to get.

```yaml
Type: String
Parameter Sets: Find by Name
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProductId
Specifies the ID of the product for which to get the API.

```yaml
Type: String
Parameter Sets: Find by product ID
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

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementApi>

## NOTES

## RELATED LINKS

[Export-AzureRmApiManagementApi](./Export-AzureRmApiManagementApi.md)

[Import-AzureRmApiManagementApi](./Import-AzureRmApiManagementApi.md)

[New-AzureRmApiManagementApi](./New-AzureRmApiManagementApi.md)

[Remove-AzureRmApiManagementApi](./Remove-AzureRmApiManagementApi.md)

[Set-AzureRmApiManagementApi](./Set-AzureRmApiManagementApi.md)


