---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Connect-ServiceFabricCluster.md
schema: 2.0.0
ms.assetid: D3EBED16-23D5-4F21-8917-21E36A6ADD78
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricClusterManifest.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricClusterManifest.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricClusterManifest

## SYNOPSIS
Gets the Service Fabric cluster manifest.

## SYNTAX

```
Get-ServiceFabricClusterManifest [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricClusterManifest** cmdlet gets the Service Fabric cluster manifest for the current connection.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Get the cluster manifest
```
PS C:\>Get-ServiceFabricClusterManifest
```

This command gets the cluster manifest for the current Service Fabric connection.

## PARAMETERS

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
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

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns a string that represents the cluster manifest.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[Test-ServiceFabricClusterManifest](./Test-ServiceFabricClusterManifest.md)


