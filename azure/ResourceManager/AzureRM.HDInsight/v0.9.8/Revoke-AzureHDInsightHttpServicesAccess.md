---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version: .\Grant-AzureHDInsightHttpServicesAccess.md
schema: 2.0.0
ms.assetid: C63357D3-BE16-4EE2-B2F1-B24EAEC21DB3
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v0.9.8/Revoke-AzureHDInsightHttpServicesAccess.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v0.9.8/Revoke-AzureHDInsightHttpServicesAccess.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Revoke-AzureHDInsightHttpServicesAccess

## SYNOPSIS
Disables HTTP access to a cluster.

## SYNTAX

```
Revoke-AzureHDInsightHttpServicesAccess [-ResourceGroupName] <String> [-ClusterName] <String>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Revoke-AzureHDInsightHttpServicesAccess** cmdlet disables HTTP access to a cluster for ODBC, Ambari, Oozie and webHCatalog web services.

## EXAMPLES

### Example 1: Disable HTTP access to a cluster
```
PS C:\> # Cluster info
        $clusterResourceGroupName = "Group"
        $clusterName = "your-hadoop-001"

        Revoke-AzureHDInsightHttpServicesAccess `
            -ResourceGroupName $clusterResourceGroupName `
            -ClusterName $clusterName
```

## PARAMETERS

### -ClusterName
Gets or sets the name of the cluster.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### -ResourceGroupName
Gets or sets the name of the resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
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

[Grant-AzureHDInsightHttpServicesAccess](./Grant-AzureHDInsightHttpServicesAccess.md)

[Azure HDInsight Cmdlets](./AzureRM.HDInsight.md)


