---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/18/2016 3:10 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/ServiceFabric/v3.1/Register-ServiceFabricClusterPackage.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/64b91ee622d0b9ae6539db10e927e50881fae64d/ServiceFabric/v3.1/Register-ServiceFabricClusterPackage.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Register-ServiceFabricClusterPackage

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### Both (Default)
```
Register-ServiceFabricClusterPackage -CodePackagePath <String> -ClusterManifestPath <String>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Code
```
Register-ServiceFabricClusterPackage [-Code] -CodePackagePath <String> [-ClusterManifestPath <String>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Config
```
Register-ServiceFabricClusterPackage [-Config] [-CodePackagePath <String>] -ClusterManifestPath <String>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ClusterManifestPath
{{Fill ClusterManifestPath Description}}

```yaml
Type: String
Parameter Sets: Both, Config
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Code
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Code
{{Fill Code Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Code
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CodePackagePath
{{Fill CodePackagePath Description}}

```yaml
Type: String
Parameter Sets: Both, Code
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Config
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Config
{{Fill Config Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Config
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
{{Fill TimeoutSec Description}}

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

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

