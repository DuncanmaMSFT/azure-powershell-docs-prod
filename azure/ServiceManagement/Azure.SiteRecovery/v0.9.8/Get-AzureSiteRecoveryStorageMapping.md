---
external help file: Microsoft.Azure.Commands.RecoveryServices.dll-Help.xml
online version: .\New-AzureSiteRecoveryStorageMapping.md
schema: 2.0.0
ms.assetid: 43B771B6-AD59-4C14-9BDF-5416BF33F478
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v0.9.8/Get-AzureSiteRecoveryStorageMapping.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v0.9.8/Get-AzureSiteRecoveryStorageMapping.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureSiteRecoveryStorageMapping

## SYNOPSIS
Gets mappings of Azure Site Recovery Storage objects for the current vault.

## SYNTAX

```
Get-AzureSiteRecoveryStorageMapping -PrimaryServer <ASRServer> -RecoveryServer <ASRServer>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSiteRecoveryStorageMapping** cmdlet gets mappings of Azure Site Recovery Storage objects for the current Azure Site Recovery vault.

## EXAMPLES

### Example 1: Get the mapping between a Storage object and a recovery Storage object
```
PS C:\>$Servers = Get-AzureSiteRecoveryServer
PS C:\> Get-AzureSiteRecoveryStorageMapping -PrimaryServer $Servers[0] -RecoveryServer $Servers[1]
PrimaryServerId     : 774859b0-1966-48cc-9df7-759c441b7a8c
PrimaryStorageId    : 1c1d0c0b-0c50-4675-af1a-1fdac70dbb6d
PrimaryStorageName  : phase2PrimaryStorageClassification
RecoveryServerId    : 774859b0-1966-48cc-9df7-759c441b7a8c
RecoveryStorageId   : 20cf8d92-fd5d-4872-985a-0f4562b8a0bf
RecoveryStorageName : phase2RecoveryStorageClassification
```

The first command cmdlet gets servers for the current Azure Site Recovery vault by using the **Get-AzureSiteRecoveryServer** cmdlet.
The command stores the Microsoft Azure Site Recovery servers in the $Servers array variable.

The second command gets the mapping between two Azure Storage objects.
The command specifies the primary server for the Storage object mapping as the first element of $Servers.
The command specifies the server for the recovery Storage object as the second element of $Servers.

## PARAMETERS

### -PrimaryServer
Specifies the primary Azure Site Recovery Storage object.
To obtain a server, use the **Get-AzureSiteRecoveryServer** cmdlet.

```yaml
Type: ASRServer
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecoveryServer
Specifies the recovery server.
To obtain a server, use the **Get-AzureSiteRecoveryServer** cmdlet.

```yaml
Type: ASRServer
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies an Azure profile.

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

## NOTES

## RELATED LINKS

[New-AzureSiteRecoveryStorageMapping](./New-AzureSiteRecoveryStorageMapping.md)

[Remove-AzureSiteRecoveryStorageMapping](./Remove-AzureSiteRecoveryStorageMapping.md)

[Get-AzureSiteRecoveryServer](./Get-AzureSiteRecoveryServer.md)


