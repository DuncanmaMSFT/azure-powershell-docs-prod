---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 4fd915d4-c8ad-486e-9162-a6ec3864d7e6
schema: 2.0.0
ms.assetid: CBDE7141-7332-4884-A0F9-2E5D3A4D76BD
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Add-AzureInternalLoadBalancer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Add-AzureInternalLoadBalancer.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureInternalLoadBalancer

## SYNOPSIS
Adds an internal load balancer to an Azure service.

## SYNTAX

### ServiceAndSlot (Default)
```
Add-AzureInternalLoadBalancer [-InternalLoadBalancerName] <String> [-ServiceName] <String>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### SubnetNameOnly
```
Add-AzureInternalLoadBalancer [-InternalLoadBalancerName] <String> [-ServiceName] <String>
 [-SubnetName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### SubnetNameAndIP
```
Add-AzureInternalLoadBalancer [-InternalLoadBalancerName] <String> [-ServiceName] <String>
 [-SubnetName] <String> [-StaticVNetIPAddress] <IPAddress> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureInternalLoadBalancer** cmdlet adds an internal load balancer configuration to an Azure service.
For a virtual network, you can specify a subnet or the IP address of the internal load balancer.

## EXAMPLES

### Example 1: Add an internal load balancer
```
PS C:\>Add-AzureInternalLoadBalancer -ServiceName "ContosoWebsite01" -InternalLoadBalancerName "ContosoILB"
```

This command adds an internal load balancer named ContosoILB to the service named ContosoWebsite01.

### Example 2: Add an internal load balancer for a specified subnet
```
PS C:\>Add-AzureInternalLoadBalancer -ServiceName "ContosoWebsite01" -InternalLoadBalancerName "ContosoILB" -SubnetName "FrontEndSubnet"
```

This command adds an internal load balancer named ContosoILB to the service named ContosoWebsite01.
The command specifies the subnet named FrontEndSubnet.

### Example 3: Add an internal load balancer for a specified subnet and address
```
PS C:\>Add-AzureInternalLoadBalancer -ServiceName "ContosoWebsite01" -InternalLoadBalancerName "ContosoILB" -SubnetName "FrontEndSubnet" -StaticVNetIPAddress 192.168.4.7
```

This command adds an internal load balancer named ContosoILB to the service named ContosoWebsite01.
The command specifies the subnet named FrontEndSubnet and the static address of the virtual network.

## PARAMETERS

### -InternalLoadBalancerName
Specifies the name of the internal load balancer that this cmdlet adds.

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

### -ServiceName
Specifies the name of the service to which this cmdlet adds an internal load balancer.

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

### -SubnetName
Specifies the name of the subnet for an internal load balancer that this cmdlet adds.

```yaml
Type: String
Parameter Sets: SubnetNameOnly, SubnetNameAndIP
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StaticVNetIPAddress
Specifies the virtual network IP address for an internal load balancer that this cmdlet adds.

```yaml
Type: IPAddress
Parameter Sets: SubnetNameAndIP
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.WindowsAzure.Commands.Utilities.Common.ManagementOperationContext

## NOTES

## RELATED LINKS

[Get-AzureInternalLoadBalancer](./Get-AzureInternalLoadBalancer.md)

[New-AzureInternalLoadBalancerConfig](./New-AzureInternalLoadBalancerConfig.md)

[Remove-AzureInternalLoadBalancer](./Remove-AzureInternalLoadBalancer.md)

[Set-AzureInternalLoadBalancer](./Set-AzureInternalLoadBalancer.md)


