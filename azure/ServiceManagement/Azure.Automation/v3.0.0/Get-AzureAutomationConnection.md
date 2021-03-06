---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: 7d9ec421-8039-4c36-ac81-613bff1fc2c6
schema: 2.0.0
ms.assetid: 98D08DBC-491F-4693-AFD2-D07A8AD50F32
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationConnection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationConnection.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureAutomationConnection

## SYNOPSIS
Gets an Azure Automation connection.

## SYNTAX

### ByAll (Default)
```
Get-AzureAutomationConnection [-AutomationAccountName] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

### ByConnectionName
```
Get-AzureAutomationConnection -Name <String> [-AutomationAccountName] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

### ByConnectionTypeName
```
Get-AzureAutomationConnection -ConnectionTypeName <String> [-AutomationAccountName] <String>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureAutomationConnection** cmdlet gets one or more Microsoft Azure Automation connections.
By default, all connections are returned.
To get a specific connection, specify its name.
To get all connections of a certain type, specify the connection type name.

## EXAMPLES

### Example 1: Get all connections
```
PS C:\>Get-AzureAutomationConnection -AutomationAccountName "Contoso17"
```

This command gets all connections in the Automation account named Contoso17.

### Example 2: Get all connections of a type
```
PS C:\>Get-AzureAutomationConnection -AutomationAccountName "Contoso17"  ¢â‚¬"ConnectionTypeName "Azure"
```

This command gets all Azure connections in the Automation account named Contoso17.

### Example 3: Get a connection
```
PS C:\>Get-AzureAutomationConnection -AutomationAccountName "Contoso17"  ¢â‚¬"Name "Azure"
```

This command gets the connection named MyConnection.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the automation account with the connection to retrieve.

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

### -ConnectionTypeName
Specifies the name of a connection type for the connections to retrieve.

```yaml
Type: String
Parameter Sets: ByConnectionTypeName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of a connection to retrieve.

```yaml
Type: String
Parameter Sets: ByConnectionName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
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

### Microsoft.Azure.Commands.Automation.Model.Connection

## NOTES

## RELATED LINKS

[New-AzureAutomationConnection](./New-AzureAutomationConnection.md)

[Remove-AzureAutomationConnection](./Remove-AzureAutomationConnection.md)

[Set-AzureAutomationConnectionFieldValue](./Set-AzureAutomationConnectionFieldValue.md)


