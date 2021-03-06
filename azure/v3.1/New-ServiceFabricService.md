---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/18/2016 3:10 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/ServiceFabric/v3.1/New-ServiceFabricService.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/64b91ee622d0b9ae6539db10e927e50881fae64d/ServiceFabric/v3.1/New-ServiceFabricService.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-ServiceFabricService

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### Stateless Singleton Non-Adhoc (Default)
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeSingleton] [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -InstanceCount <Int32> [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful Named Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeNamed] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionNames <String[]> [-HasPersistedState] -TargetReplicaSetSize <Int32>
 -MinReplicaSetSize <Int32> [-ReplicaRestartWaitDuration <TimeSpan>] [-QuorumLossWaitDuration <TimeSpan>]
 [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful Singleton Non-Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeSingleton] [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> [-HasPersistedState] -TargetReplicaSetSize <Int32> -MinReplicaSetSize <Int32>
 [-ReplicaRestartWaitDuration <TimeSpan>] [-QuorumLossWaitDuration <TimeSpan>]
 [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful UniformInt64 Non-Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeUniformInt64] [-ApplicationName] <Uri>
 [-ServiceName] <Uri> [-ServiceTypeName] <String> -PartitionCount <Int32> -LowKey <Int64> -HighKey <Int64>
 [-HasPersistedState] -TargetReplicaSetSize <Int32> -MinReplicaSetSize <Int32>
 [-ReplicaRestartWaitDuration <TimeSpan>] [-QuorumLossWaitDuration <TimeSpan>]
 [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful Named Non-Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeNamed] [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionNames <String[]> [-HasPersistedState] -TargetReplicaSetSize <Int32>
 -MinReplicaSetSize <Int32> [-ReplicaRestartWaitDuration <TimeSpan>] [-QuorumLossWaitDuration <TimeSpan>]
 [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful Singleton Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeSingleton] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> [-HasPersistedState] -TargetReplicaSetSize <Int32> -MinReplicaSetSize <Int32>
 [-ReplicaRestartWaitDuration <TimeSpan>] [-QuorumLossWaitDuration <TimeSpan>]
 [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateful UniformInt64 Adhoc
```
New-ServiceFabricService [-Stateful] [-PartitionSchemeUniformInt64] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionCount <Int32> -LowKey <Int64> -HighKey <Int64> [-HasPersistedState]
 -TargetReplicaSetSize <Int32> -MinReplicaSetSize <Int32> [-ReplicaRestartWaitDuration <TimeSpan>]
 [-QuorumLossWaitDuration <TimeSpan>] [-StandByReplicaKeepDuration <TimeSpan>] [-PlacementConstraint <String>]
 [-Metric <String[]>] [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Stateless UniformInt64 Adhoc
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeUniformInt64] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionCount <Int32> -LowKey <Int64> -HighKey <Int64> -InstanceCount <Int32>
 [-PlacementConstraint <String>] [-Metric <String[]>] [-Correlation <String[]>] [-PlacementPolicy <String[]>]
 [-DefaultMoveCost <String>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Stateless Named Adhoc
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeNamed] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionNames <String[]> -InstanceCount <Int32> [-PlacementConstraint <String>]
 [-Metric <String[]>] [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Stateless Named Non-Adhoc
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeNamed] [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -PartitionNames <String[]> -InstanceCount <Int32> [-PlacementConstraint <String>]
 [-Metric <String[]>] [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Stateless Singleton Adhoc
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeSingleton] [-Adhoc] [-ServiceName] <Uri>
 [-ServiceTypeName] <String> -InstanceCount <Int32> [-PlacementConstraint <String>] [-Metric <String[]>]
 [-Correlation <String[]>] [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Stateless UniformInt64 Non-Adhoc
```
New-ServiceFabricService [-Stateless] [-PartitionSchemeUniformInt64] [-ApplicationName] <Uri>
 [-ServiceName] <Uri> [-ServiceTypeName] <String> -PartitionCount <Int32> -LowKey <Int64> -HighKey <Int64>
 -InstanceCount <Int32> [-PlacementConstraint <String>] [-Metric <String[]>] [-Correlation <String[]>]
 [-PlacementPolicy <String[]>] [-DefaultMoveCost <String>] [-TimeoutSec <Int32>] [<CommonParameters>]
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

### -Adhoc
{{Fill Adhoc Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc, Stateless UniformInt64 Adhoc, Stateless Named Adhoc, Stateless Singleton Adhoc
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationName
{{Fill ApplicationName Description}}

```yaml
Type: Uri
Parameter Sets: Stateless Singleton Non-Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateless Named Non-Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Correlation
{{Fill Correlation Description}}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultMoveCost
{{Fill DefaultMoveCost Description}}

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

### -HasPersistedState
{{Fill HasPersistedState Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HighKey
{{Fill HighKey Description}}

```yaml
Type: Int64
Parameter Sets: Stateful UniformInt64 Non-Adhoc, Stateful UniformInt64 Adhoc, Stateless UniformInt64 Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceCount
{{Fill InstanceCount Description}}

```yaml
Type: Int32
Parameter Sets: Stateless Singleton Non-Adhoc, Stateless UniformInt64 Adhoc, Stateless Named Adhoc, Stateless Named Non-Adhoc, Stateless Singleton Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LowKey
{{Fill LowKey Description}}

```yaml
Type: Int64
Parameter Sets: Stateful UniformInt64 Non-Adhoc, Stateful UniformInt64 Adhoc, Stateless UniformInt64 Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Metric
{{Fill Metric Description}}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MinReplicaSetSize
{{Fill MinReplicaSetSize Description}}

```yaml
Type: Int32
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionCount
{{Fill PartitionCount Description}}

```yaml
Type: Int32
Parameter Sets: Stateful UniformInt64 Non-Adhoc, Stateful UniformInt64 Adhoc, Stateless UniformInt64 Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionNames
{{Fill PartitionNames Description}}

```yaml
Type: String[]
Parameter Sets: Stateful Named Adhoc, Stateful Named Non-Adhoc, Stateless Named Adhoc, Stateless Named Non-Adhoc
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionSchemeNamed
{{Fill PartitionSchemeNamed Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateful Named Adhoc, Stateful Named Non-Adhoc, Stateless Named Adhoc, Stateless Named Non-Adhoc
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionSchemeSingleton
{{Fill PartitionSchemeSingleton Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateless Singleton Non-Adhoc, Stateful Singleton Non-Adhoc, Stateful Singleton Adhoc, Stateless Singleton Adhoc
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionSchemeUniformInt64
{{Fill PartitionSchemeUniformInt64 Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateful UniformInt64 Non-Adhoc, Stateful UniformInt64 Adhoc, Stateless UniformInt64 Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PlacementConstraint
{{Fill PlacementConstraint Description}}

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

### -PlacementPolicy
{{Fill PlacementPolicy Description}}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -QuorumLossWaitDuration
{{Fill QuorumLossWaitDuration Description}}

```yaml
Type: TimeSpan
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicaRestartWaitDuration
{{Fill ReplicaRestartWaitDuration Description}}

```yaml
Type: TimeSpan
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
{{Fill ServiceName Description}}

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceTypeName
{{Fill ServiceTypeName Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StandByReplicaKeepDuration
{{Fill StandByReplicaKeepDuration Description}}

```yaml
Type: TimeSpan
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Stateful
{{Fill Stateful Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Stateless
{{Fill Stateless Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Stateless Singleton Non-Adhoc, Stateless UniformInt64 Adhoc, Stateless Named Adhoc, Stateless Named Non-Adhoc, Stateless Singleton Adhoc, Stateless UniformInt64 Non-Adhoc
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetReplicaSetSize
{{Fill TargetReplicaSetSize Description}}

```yaml
Type: Int32
Parameter Sets: Stateful Named Adhoc, Stateful Singleton Non-Adhoc, Stateful UniformInt64 Non-Adhoc, Stateful Named Non-Adhoc, Stateful Singleton Adhoc, Stateful UniformInt64 Adhoc
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

