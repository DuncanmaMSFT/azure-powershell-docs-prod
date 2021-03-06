---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
online version: 07cdf07f-d115-4450-ae3c-2915ba1e5b8d
schema: 2.0.0
ms.assetid: 0892A13C-5B63-46F7-A502-5BB92EEE211A
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v1.0/Set-AzureRmTrafficManagerEndpoint.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v1.0/Set-AzureRmTrafficManagerEndpoint.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Set-AzureRmTrafficManagerEndpoint

## SYNOPSIS
Updates a Traffic Manager endpoint.

## SYNTAX

```
Set-AzureRmTrafficManagerEndpoint -TrafficManagerEndpoint <TrafficManagerEndpoint> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmTrafficManagerEndpoint** cmdlet updates an endpoint in azure_2 Traffic Manager.
This cmdlet updates the settings from a local endpoint object.
You can specify the endpoint object either by using the *TrafficManagerEndpoint* parameter or by using the pipeline.

You can obtain a local object that represents an endpoint by using the Get-AzureRmTrafficManagerEndpoint cmdlet.
Modify the object locally and then use **Set-AzureRmTrafficManagerEndpoint** to commit your changes.

## EXAMPLES

### Example 1: Update an endpoint
```
PS C:\>$TrafficManagerEndpoint = Get-AzureRmTrafficManagerEndpoint -Name "endpoint1" -Type AzureEndpoints -ProfileName "ContosoProfile" -ResourceGroupName "ResourceGroup11"
PS C:\> $TrafficManagerEndpoint.Weight = 20
PS C:\> Set-AzureRmTrafficManagerEndpoint -TrafficManagerEndpoint $TrafficManagerEndpoint
```

The first command gets an azure_2 Traffic Manager endpoint by using the **Get-AzureRmTrafficManagerEndpoint** cmdlet.
The command stores the endpoint locally in the $TrafficManagerEndpoint variable.

The second command changes that endpoint locally.
This command changes the endpoint weight to 20.

The third command updates the endpoint in Traffic Manager to match the local value in $TrafficManagerEndpoint.

## PARAMETERS

### -TrafficManagerEndpoint
Specifies a local **TrafficManagerEndpoint** object.
This cmdlet updates Traffic Manager to match this local object.

```yaml
Type: TrafficManagerEndpoint
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Network.TrafficManagerEndpoint
This cmdlet accepts a **TrafficManagerEndpoint** object.

## OUTPUTS

### Microsoft.Azure.Commands.Network.TrafficManagerEndpoint
This cmdlet returns a **TrafficManagerEndpoint** object.

## NOTES

## RELATED LINKS


