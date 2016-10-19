---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
online version: .\Disable-AzureRmTrafficManagerEndpoint.md
schema: 2.0.0
ms.assetid: C6E4F727-AC36-4165-9298-BF51ABA716DD
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.1.0/Get-AzureRmTrafficManagerEndpoint.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.1.0/Get-AzureRmTrafficManagerEndpoint.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmTrafficManagerEndpoint

## SYNOPSIS
Gets an endpoint for a Traffic Manager profile.

## SYNTAX

### Fields
```
Get-AzureRmTrafficManagerEndpoint -Name <String> -Type <String> -ProfileName <String>
 -ResourceGroupName <String> [<CommonParameters>]
```

### Object
```
Get-AzureRmTrafficManagerEndpoint -TrafficManagerEndpoint <TrafficManagerEndpoint> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmTrafficManagerEndpoint** cmdlet gets an endpoint for an Azure Traffic Manager profile.

You can modify this object locally, and then apply changes to the profile by using the Set-AzureRmTrafficManagerEndpoint cmdlet.
Specify the endpoint by using the *Name* and *Type* parameters.
You can specify the Traffic Manager profile either by using the *ProfileName* and *ResourceGroupName* parameter, or by specifying a **TrafficManagerProfile** object.
Alternatively, you can pass that value by using the pipeline.

## EXAMPLES

### Example 1: Get an endpoint
```
PS C:\>$TrafficManagerEndpoint = Get-AzureRmTrafficManagerEndpoint -Name "contoso" -ProfileName "ContosoProfile" -ResourceGroupName "ResourceGroup11" -Type AzureEndpoints
```

This command gets the Azure endpoint named contoso from the profile named ContosoProfile in the resource group named ResourceGroup11, and then stores that object in the $TrafficManagerEndpoint variable.

## PARAMETERS

### -Name
Specifies the name of the Traffic Manager endpoint that this cmdlet gets.

```yaml
Type: String
Parameter Sets: Fields
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProfileName
Specifies the name of the Traffic Manager endpoint that this cmdlet gets.

```yaml
Type: String
Parameter Sets: Fields
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet gets a Traffic Manager endpoint in the group that this parameter specifies.

```yaml
Type: String
Parameter Sets: Fields
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TrafficManagerEndpoint
Specifies the Traffic Manager endpoint that this cmdlet gets.

```yaml
Type: TrafficManagerEndpoint
Parameter Sets: Object
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Type
Specifies the type of endpoint that this cmdlet adds to the Traffic Manager profile.
Valid values are: 

- AzureEndpoints
- ExternalEndpoints
- NestedEndpoints

```yaml
Type: String
Parameter Sets: Fields
Aliases: 
Accepted values: AzureEndpoints, ExternalEndpoints, NestedEndpoints

Required: True
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

[Disable-AzureRmTrafficManagerEndpoint](.\Disable-AzureRmTrafficManagerEndpoint.md)

[Enable-AzureRmTrafficManagerEndpoint](.\Enable-AzureRmTrafficManagerEndpoint.md)

[New-AzureRmTrafficManagerEndpoint](.\New-AzureRmTrafficManagerEndpoint.md)

[Remove-AzureRmTrafficManagerEndpoint](.\Remove-AzureRmTrafficManagerEndpoint.md)

[Set-AzureRmTrafficManagerEndpoint](.\Set-AzureRmTrafficManagerEndpoint.md)

