---
external help file: Microsoft.Azure.Commands.NotificationHubs.dll-Help.xml
online version: .\Get-AzureRmNotificationHub.md
schema: 2.0.0
ms.assetid: 8DDCE5B2-E8EB-48C6-8ACE-9DA062E10303
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v1.0.12/New-AzureRmNotificationHub.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v1.0.12/New-AzureRmNotificationHub.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmNotificationHub

## SYNOPSIS
Creates a notification hub.

## SYNTAX

### InputFileParameterSet
```
New-AzureRmNotificationHub [-ResourceGroup] <String> [-Namespace] <String> [-InputFile] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### NotificationHubParameterSet
```
New-AzureRmNotificationHub [-ResourceGroup] <String> [-Namespace] <String>
 [-NotificationHubObj] <NotificationHubAttributes> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmNotificationHub** cmdlet creates a notification hub.
Notification hubs are used to send push notifications to multiple clients regardless of the platform used by those clients.
Notification hubs are roughly equivalent to individual apps: each of your apps will typically have its own notification hub.

The **New-AzureRmNotificationHub** cmdlet provides two ways to create a new notification hub.
You can create an instance of the **NotificationHubAttributes** object and then configure that object.
You can then copy those property values to your new hub by through the *NotificationHubObj* parameter.

Alternatively, you can create a JSON (JavaScript Object Notation) file containing the relevant configuration values and  then apply those values by using the *InputFile* parameter.

When used in conjunction with the **New-AzureRmNotificationHub** cmdlet, the preceding JSON sample creates a notification hub named ContosoNotificationHub located on the West US datacenter.

## EXAMPLES

### Example 1: Create a notification hub
```
PS C:\>New-AzureRmNotificationHub -Namespace "ContosoNamespace" -ResourceGroup "ContosoNotificationsGroup" -InputFile "C:\Configurations\InternalHub.json"
```

This command creates a notification hub in the namespace ContosoNamespace.
The new hub will be assigned to the ContosoNotificationsGroup.
You do not need to specify a name or any other configuration information for the hub; that information will be taken from the input file C:\Configurations\InternalHub.json.

## PARAMETERS

### -ResourceGroup
Specifies the resource group to which the notification hub will be assigned.
Resource groups organize items such as namespaces, notification hubs, and authorization rules in ways that help simply inventory management and azure_2 administration.

You must use an existing resource group.
The **New-AzureRmNotificationHub** cmdlet cannot create a new resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Namespace
Specifies the namespace to which the notification hub will be assigned.

Namespaces provide a way to group and categorize notification hubs.
Notification hubs must be assigned to an existing namespace.
The **New-AzureRmNotificationHub** cmdlet cannot create a new namespace.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InputFile
Specifies the path to a JSON file containing configuration values for the new notification hub.

```yaml
Type: String
Parameter Sets: InputFileParameterSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotificationHubObj
Specifies the **NotificationHubAttributes** object that contains configuration information for the new hub.

```yaml
Type: NotificationHubAttributes
Parameter Sets: NotificationHubParameterSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
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

## NOTES

## RELATED LINKS

[Get-AzureRmNotificationHub](./Get-AzureRmNotificationHub.md)

[Remove-AzureRmNotificationHub](./Remove-AzureRmNotificationHub.md)

[Set-AzureRmNotificationHub](./Set-AzureRmNotificationHub.md)


