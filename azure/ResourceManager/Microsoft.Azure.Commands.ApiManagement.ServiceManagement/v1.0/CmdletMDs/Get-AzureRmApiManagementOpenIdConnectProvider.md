---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: .\New-AzureRmApiManagementOpenIdConnectProvider.md
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.0/CmdletMDs/Get-AzureRmApiManagementOpenIdConnectProvider.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v1.0/CmdletMDs/Get-AzureRmApiManagementOpenIdConnectProvider.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# Get-AzureRmApiManagementOpenIdConnectProvider

## SYNOPSIS
Gets OpenID Connect providers.

## SYNTAX

### Get all OpenID Connect Providers (Default)
```
Get-AzureRmApiManagementOpenIdConnectProvider -Context <PsApiManagementContext>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Get by OpenID Connect Provider ID
```
Get-AzureRmApiManagementOpenIdConnectProvider -Context <PsApiManagementContext>
 [-OpenIdConnectProviderId <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

### Find by OpenID Connect Provider friendly Name
```
Get-AzureRmApiManagementOpenIdConnectProvider -Context <PsApiManagementContext> [-Name <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApiManagementOpenIdConnectProvider** cmdlet gets OpenID Connect providers in azure_2 API Management.

## EXAMPLES

### Example 1: Get all providers
```
PS C:\>Get-AzureRmApiManagementOpenIdConnectProvider -Context $ApimContext
```

This command gets all OpenID Connect providers for the specified context.

### Example 2: Get a provider by using an ID
```
PS C:\>Get-AzureRmApiManagementOpenIdConnectProvider -Context $ApimContext -OpenIdConnectProviderId "OICProvicer01"
```

This command gets the provider that has the ID OICProvicer01.

### Example 3: Get a provider by using a name
```
PS C:\>Get-AzureRmApiManagementOpenIdConnectProvider -Context $ApimContext -Name "Contoso OpenID Connect Provider"
```

This command gets the provider named Contoso OpenID Connect Provider.

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
@{Text=}```yaml
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
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OpenIdConnectProviderId
Specifies an ID of the provider that this cmdlet removes.
If you specify an ID, this cmdlet gets that provider.

```yaml
Type: String
Parameter Sets: Get by OpenID Connect Provider ID
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies a friendly name of a provider.
If you specify a name, this cmdlet gets that provider.

```yaml
Type: String
Parameter Sets: Find by OpenID Connect Provider friendly Name
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

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementOpenIdConnectProvider>

## NOTES

## RELATED LINKS

[New-AzureRmApiManagementOpenIdConnectProvider](.\New-AzureRmApiManagementOpenIdConnectProvider.md)

[Remove-AzureRmApiManagementOpenIdConnectProvider](.\Remove-AzureRmApiManagementOpenIdConnectProvider.md)

[Set-AzureRmApiManagementOpenIdConnectProvider](.\Set-AzureRmApiManagementOpenIdConnectProvider.md)
