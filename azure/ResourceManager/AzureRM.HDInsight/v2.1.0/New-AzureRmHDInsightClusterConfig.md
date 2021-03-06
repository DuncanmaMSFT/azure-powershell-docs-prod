---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version: .\Add-AzureRmHDInsightStorage.md
schema: 2.0.0
ms.assetid: 66213503-6FA4-49BB-B932-945C4BB9BB34
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.1.0/New-AzureRmHDInsightClusterConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.1.0/New-AzureRmHDInsightClusterConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmHDInsightClusterConfig

## SYNOPSIS
Creates a non-persisted cluster configuration object that describes an Azure HDInsight cluster configuration.

## SYNTAX

```
New-AzureRmHDInsightClusterConfig [-DefaultStorageAccountName <String>] [-DefaultStorageAccountKey <String>]
 [-OozieMetastore <AzureHDInsightMetastore>] [-HiveMetastore <AzureHDInsightMetastore>]
 [-HeadNodeSize <String>] [-WorkerNodeSize <String>] [-ZookeeperNodeSize <String>] [-ClusterType <String>]
 [-ClusterTier <Tier>] [-ObjectId <Guid>] [-CertificateFileContents <Byte[]>] [-CertificateFilePath <String>]
 [-CertificatePassword <String>] [-AadTenantId <Guid>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmHDInsightClusterConfig** cmdlet creates a non-persisted object that describes an Azure HDInsight cluster configuration.

## EXAMPLES

### Example 1: Create a cluster configuration object
```
PS C:\># Primary storage account info
PS C:\> $storageAccountResourceGroupName = "Group"
PS C:\> $storageAccountName = "yourstorageacct001"
PS C:\> $storageAccountKey = (Get-AzureRmStorageAccountKey -ResourceGroupName $storageAccountResourceGroupName -Name $storageAccountName)[0].value


PS C:\> $storageContainer = "container002"

# Cluster configuration info
PS C:\> $location = "East US 2"
PS C:\> $clusterResourceGroupName = "Group"
PS C:\> $clusterName = "your-hadoop-002"
PS C:\> $clusterCreds = Get-Credential

# If the cluster's resource group doesn't exist yet, run:
#   New-AzureRmResourceGroup -Name $clusterResourceGroupName -Location $location

# Create the cluster
PS C:\> New-AzureRmHDInsightClusterConfig `
            | Add-AzureRmHDInsightStorage `
                -StorageAccountName "$secondStorageAccountName.blob.core.contoso.net" `
                -StorageAccountKey $key2 `
            | New-AzureRmHDInsightCluster `
                -ClusterType Hadoop `
                -OSType Windows `
                -ClusterSizeInNodes 4 `
                -ResourceGroupName $clusterResourceGroupName `
                -ClusterName $clusterName `
                -HttpCredential $clusterCreds `
                -Location $location `
                -DefaultStorageAccountName "$storageAccountName.blob.core.contoso.net" `
                -DefaultStorageAccountKey $storageAccountKey `
                -DefaultStorageContainer $storageContainer
```

This command creates a cluster configuration object.

## PARAMETERS

### -DefaultStorageAccountName
Specifies the name of the default storage account that the HDInsight cluster will use.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultStorageAccountKey
Specifies the account key for the default Azure Storage account that the HDInsight cluster will use.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OozieMetastore
Specifies the metastore to store Oozie metadata.
You can alternatively use the **Add-AzureRmHDInsightMetastore** cmdlet.

```yaml
Type: AzureHDInsightMetastore
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HiveMetastore
Specifies the metastore to store Hive metadata.
You can alternatively use the Add-AzureRmHDInsightMetastore cmdlet.

```yaml
Type: AzureHDInsightMetastore
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HeadNodeSize
Specifies the size of the virtual machine for the Head node.
Use Get-AzureRMVMSize for acceptable VM sizes, and see HDInsight's pricing page.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkerNodeSize
Specifies the size of the virtual machine for the Worker node.
Use Get-AzureRMVMSize for acceptable VM sizes, and see HDInsight's pricing page.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ZookeeperNodeSize
Specifies the size of the virtual machine for the Zookeeper node.
Use Get-AzureRMVMSize for acceptable VM sizes, and see HDInsight's pricing page.
This parameter is valid only for HBase or Storm clusters.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClusterType
Specifies the type of cluster to create.
The acceptable values for this parameter are:

- Hadoop
- HBase
- Storm
- Spark

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClusterTier
Specifies the HDInsight cluster tier.
The acceptable values for this parameter are:

- Standard
- Premium

The default value is Standard.
The Premium tier can only be used with Linux clusters, and it enables the use of some new features.

```yaml
Type: Tier
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectId
Specifies the Azure AD object ID (a GUID) of the Azure AD Service Principal that represents the cluster.
The cluster will use this when accessing Azure Data Lake Store.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateFileContents
Specifies file contents of the certificate that will be used when accessing Azure Data Lake Store.

```yaml
Type: Byte[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateFilePath
Specifies the file path to the certificate that will be used to authenticate as the Service Principal.
The cluster will use this when accessing Azure Data Lake Store.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificatePassword
Specifies the password for the certificate that will be used to authenticate as the Service Principal.
The cluster will use this when accessing Azure Data Lake Store.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AadTenantId
Specifies the Azure AD Tenant ID that will be used when accessing Azure Data Lake Store.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
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

[Add-AzureRmHDInsightStorage](./Add-AzureRmHDInsightStorage.md)


