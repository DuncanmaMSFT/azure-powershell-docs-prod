---
external help file: Microsoft.Azure.Commands.NotificationHubs.dll-Help.xml
online version: 3d945357-195d-494d-9b14-5523655ffb04
schema: 2.0.0
ms.assetid: F167BBA1-B756-49FD-81B7-CFAFCE463593
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.2.0/Get-AzureRmNotificationHubsNamespace.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.2.0/Get-AzureRmNotificationHubsNamespace.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmNotificationHubsNamespace

## SYNOPSIS
Gets information about a notification hub namespace.

## SYNTAX

```
Get-AzureRmNotificationHubsNamespace [[-ResourceGroup] <String>] [[-Namespace] <String>] [<CommonParameters>]
```

## DESCRIPTION
**The Get-AzureRmNotificationHubsNamespace** cmdlet gets information about notification hub namespaces.
This cmdlet provides you the option of getting information for all your namespaces, information about the namespaces assigned to a specified resource group; or for returning information about a specific namespace.

Namespaces are logical containers that help you organize and manage your notification hubs.
You must have at least one notification hub namespace: all notification hubs must be assigned to a namespace.
A single namespace can house multiple hubs which means that you might only need one namespace in your organization.
However, you can also have multiple namespaces to better organize your hubs, or to give specific individuals permission to manage a selected subset of hubs.

The **Get-AzureRmNotificationHubsNamespace** cmdlet returns basic information about the namespace itself.
To get information about the authorization rules associated with a namespace use Get-AzureRmNotificationHubsNamespaceAuthorizationRules.

## EXAMPLES

### Example 1: Get information for all notification hub namespaces
```
PS C:\>Get-AzureRmNotificationHubsNamespace
```

This command returns information for all your notification hub namespaces.

### Example 2: Get information for a single notification hub namespace
```
PS C:\>Get-AzureRmNotificationHubsNamespace -Namespace "ContosoNamespace"
```

This command gets information for a single notification hub namespace: ContosoNamespace.

### Example 3: Get information for all notification hubs assigned to a specific namespace
```
PS C:\>Get-AzureRmNotificationHubsNamespace -ResourceGroup "ContosoNotificationsGroup"
```

This command gets information for all notification hub namespaces assigned to the resource group ContosoNotificationsGroup.

## PARAMETERS

### -ResourceGroup
Specifies the resource group to which the namespace is assigned.

Resource groups organize items such as namespaces, notification hubs, and authorization rules in ways that help simply inventory management and Azure administration.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Namespace
Specifies a unique name for the namespace.

Namespaces provide a way to group and categorize notification hubs.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmNotificationHubsNamespaceAuthorizationRules](./Get-AzureRmNotificationHubsNamespaceAuthorizationRules.md)

[New-AzureRmNotificationHubsNamespace](./New-AzureRmNotificationHubsNamespace.md)

[Remove-AzureRmNotificationHubsNamespace](./Remove-AzureRmNotificationHubsNamespace.md)

[Set-AzureRmNotificationHubsNamespace](./Set-AzureRmNotificationHubsNamespace.md)


