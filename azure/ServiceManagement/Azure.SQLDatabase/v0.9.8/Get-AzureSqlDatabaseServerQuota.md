---
external help file: Microsoft.WindowsAzure.Commands.SqlDatabase.dll-Help.xml
online version: .\New-AzureSqlDatabaseServerContext.md
schema: 2.0.0
ms.assetid: FE6E38A0-9B4D-40CA-994A-C2F73142ECB6
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v0.9.8/Get-AzureSqlDatabaseServerQuota.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v0.9.8/Get-AzureSqlDatabaseServerQuota.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureSqlDatabaseServerQuota

## SYNOPSIS
Gets quota information for an Azure SQL Database server.

## SYNTAX

### ByConnectionContext
```
Get-AzureSqlDatabaseServerQuota [-ConnectionContext] <IServerDataServiceContext> [[-QuotaName] <String>]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

### ByServerName
```
Get-AzureSqlDatabaseServerQuota [-ServerName] <String> [[-QuotaName] <String>] [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSqlDatabaseServerQuota** cmdlet gets the quota information for a specified instance of Azure SQL Database Server.
Specify a connection context or the server name.
If you do not specify a quota name, this cmdlet gets all the quota information for the server.

## EXAMPLES

### Example 1: Get information for a specific quota
```
PS C:\>$QuotaPremium = GetAzureSqlDatabaseServerQuota $Context -QuotaName "Premium_Databases"
```

This command gets the quota named Premium_Databases from the Azure SQL Database server specified by the connection stored in the $Context variable.

### Example 2: Get information for all quotas
```
PS C:\>$QuotaList = GetAzureSqlDatabaseServerQuota $Context
```

This command gets all quota values from the server specified by the connection $Context.

## PARAMETERS

### -ConnectionContext
Specifies the connection context of a server.

```yaml
Type: IServerDataServiceContext
Parameter Sets: ByConnectionContext
Aliases: Context

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -QuotaName
Specifies the name of the quota value that this cmdlet gets.

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

### -ServerName
Specifies the name of a server.

```yaml
Type: String
Parameter Sets: ByServerName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
In-memory profile.

```yaml
Type: AzureProfile
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

### Microsoft.WindowsAzure.Commands.SqlDatabase.Services.Server.ServerQuota[]

## NOTES
* Authentication: This cmdlet can use either SQL Server authentication or certificate-based authentication. For examples of setting up authentication, see the New-AzureSqlDatabaseServerContext cmdlet.

## RELATED LINKS

[New-AzureSqlDatabaseServerContext](./New-AzureSqlDatabaseServerContext.md)


