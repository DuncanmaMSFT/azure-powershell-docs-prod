---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Add-AzureInternalLoadBalancer.md
schema: 2.0.0
ms.assetid: 752C3DB7-9DE8-46DC-8988-CAA69F297784
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/New-AzureInternalLoadBalancerConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/New-AzureInternalLoadBalancerConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureInternalLoadBalancerConfig

## SYNOPSIS
Creates an internal load balancer configuration.

## SYNTAX

### ServiceAndSlot (Default)
```
New-AzureInternalLoadBalancerConfig [-InternalLoadBalancerName] <String> [-Profile <AzureProfile>]
 [<CommonParameters>]
```

### SubnetNameAndIP
```
New-AzureInternalLoadBalancerConfig [-InternalLoadBalancerName] <String> [-SubnetName] <String>
 [-StaticVNetIPAddress] <IPAddress> [-Profile <AzureProfile>] [<CommonParameters>]
```

### SubnetNameOnly
```
New-AzureInternalLoadBalancerConfig [-InternalLoadBalancerName] <String> [-SubnetName] <String>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureInternalLoadBalancerConfig** cmdlet creates an **InternalLoadBalancerConfig** object.
You can use an internal load balancer configuration when you create an Azure virtual machine deployment.

## EXAMPLES

### Example 1: Create an internal load balancer configuration
```
PS C:\>$IlbConfig = New-AzureInternalLoadBalancerConfig -InternalLoadBalancerName "Contoso" -SubnetName "FrontEndSubnet"
```

This command creates an internal load balancer configuration for the subnet named FrontEndSubnet.
The command stores the configuration in the $IlbConfig variable for you to use for a virtual machine deployment.

## PARAMETERS

### -InternalLoadBalancerName
Specifies the name of the internal load balancer that this cmdlet includes in the configuration.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SubnetName
Specifies the name of the subnet for an internal load balancer.

```yaml
Type: String
Parameter Sets: SubnetNameAndIP, SubnetNameOnly
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StaticVNetIPAddress
Specifies the virtual network IP address for an internal load balancer that this cmdlet includes in the configuration.

```yaml
Type: IPAddress
Parameter Sets: SubnetNameAndIP
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.WindowsAzure.Commands.ServiceManagement.Model.InternalLoadBalancerConfig

## NOTES

## RELATED LINKS

[Add-AzureInternalLoadBalancer](./Add-AzureInternalLoadBalancer.md)

[Get-AzureInternalLoadBalancer](./Get-AzureInternalLoadBalancer.md)

[Remove-AzureInternalLoadBalancer](./Remove-AzureInternalLoadBalancer.md)

[Set-AzureInternalLoadBalancer](./Set-AzureInternalLoadBalancer.md)


