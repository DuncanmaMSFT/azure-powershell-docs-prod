---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: 638b2bf6-23f8-4038-b20b-1cfabfdbf5d3
schema: 2.0.0
ms.assetid: 3B1FC41A-FA8C-4F70-BD33-A5F7914C9DA0
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v2.2.0/Add-AzureRmApiManagementUserToGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/Microsoft.Azure.Commands.ApiManagement.ServiceManagement/v2.2.0/Add-AzureRmApiManagementUserToGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureRmApiManagementUserToGroup

## SYNOPSIS
Adds a user to a group.

## SYNTAX

```
Add-AzureRmApiManagementUserToGroup -Context <PsApiManagementContext> -GroupId <String> -UserId <String>
 [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmApiManagementUserToGroup** cmdlet adds a user to a group.

## EXAMPLES

### Example 1: Add a user to a group
```
PS C:\>Add-AzureRmApiManagementUserToGroup -Context $apimContext -GroupId "0001" -UserId "0123456789"
```

This command adds an existing user to an existing group.

## PARAMETERS

### -Context
Specifies a **PsApiManagementContext** object.
This parameter is required.

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

### -GroupId
Specifies the group ID.
This parameter is required.

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

### -UserId
Specifies the user ID.
This parameter is required.

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

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
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

### Boolean

## NOTES

## RELATED LINKS

[Get-AzureRmApiManagementUser](./Get-AzureRmApiManagementUser.md)

[Remove-AzureRmApiManagementUserFromGroup](./Remove-AzureRmApiManagementUserFromGroup.md)


