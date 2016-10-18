---
external help file: Microsoft.Azure.SqlDatabase.Jobs.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/18/2016 6:38 AM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-elasticdb/blob/master/ElasticDB/ElasticDatabaseJobs/v0.8.33/Remove-AzureSqlJobChildTarget.md
gitcommit: https://github.com/Azure/azure-docs-powershell-elasticdb/blob/0499f7a103ac6ce909eab6e4e8e3f759b6f634fe/ElasticDB/ElasticDatabaseJobs/v0.8.33/Remove-AzureSqlJobChildTarget.md
ms.topic: reference
ms.prod: powershell
ms.service: AzureAD
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureSqlJobChildTarget

## SYNOPSIS
Removes a child target from another target.

## SYNTAX

### TargetId (Default)
```
Remove-AzureSqlJobChildTarget -CustomCollectionName <String> -TargetId <Guid[]>
 [[-AzureSqlJobConnection] <AzureSqlJobConnection>] [<CommonParameters>]
```

### Database
```
Remove-AzureSqlJobChildTarget -CustomCollectionName <String> -ServerName <String[]> -DatabaseName <String[]>
 [-LiteralServerName] [[-AzureSqlJobConnection] <AzureSqlJobConnection>] [<CommonParameters>]
```

## DESCRIPTION
The Remove-AzureSqlJobChildTarget cmdlet removes a child target from another target. 
This cmdlet removes the child target from a custom collection, but it does not delete the target.

## EXAMPLES

### Example 1: Remove a database target as a child target from a custom collection
```
PS C:\>Remove-AzureSqlJobChildTarget -CustomCollectionName "MyCustomCollection" -ServerName "MyServer.database.contoso.net" -DatabaseName "MyDatabase"
```

This command removes the database target named MyServer.database.contoso.net as a child target from the custom collection named MyCustomCollection.

## PARAMETERS

### -AzureSqlJobConnection
Specifies the connection state object for the job.
You can get the connection state object through the New-AzureSqlJobConnection cmdlet.
If you do not specify this parameter, the connection state is used from a prior call to the Use-AzureSqlJobConnection cmdlet.

```yaml
Type: AzureSqlJobConnection
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomCollectionName
Specifies the name of the custom collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DatabaseName
Specifies an array that contains the database name of the database target to remove from the custom collection.

```yaml
Type: String[]
Parameter Sets: Database
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServerName
Specifies an array that contains the database server name of the database target to remove from the custom collection.

```yaml
Type: String[]
Parameter Sets: Database
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetId
Specifies an array of GUIDs that contains the target ID to remove from the custom collection.

```yaml
Type: Guid[]
Parameter Sets: TargetId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -LiteralServerName
{{Fill LiteralServerName Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Database
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

## NOTES

## RELATED LINKS

[Add-AzureSqlJobChildTarget]()

[New-AzureSqlJobConnection]()

[Use-AzureSqlJobConnection]()

[Elastic Database Jobs]()
