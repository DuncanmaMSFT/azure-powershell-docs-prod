---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
online version: .\Get-AzureBatchTask.md
schema: 2.0.0
ms.assetid: 17C6284F-05D2-4CE1-8523-E293649344AF
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.1.0/Set-AzureBatchTask.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.1.0/Set-AzureBatchTask.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureBatchTask

## SYNOPSIS
Updates the properties of a task.

## SYNTAX

```
Set-AzureBatchTask [-Task] <PSCloudTask> -BatchContext <BatchAccountContext> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureBatchTask** cmdlet updates the properties of a task in the Azure Batch service.
Use the Get-AzureBatchTask cmdlet to get a **PSCloudTask** object.
Modify the properties of that object, and then use the current cmdlet to commit your changes to the Batch service.

## EXAMPLES

### Example 1: Update a task
```
PS C:\>$Task = Get-AzureBatchTask -JobId "Job16" -Id "Task22" -BatchContext $Context
PS C:\> $Constraints = New-Object Microsoft.Azure.Commands.Batch.Models.PSTaskConstraints -ArgumentList @([TimeSpan}::FromDays(5), [TimeSpan]::FromDays(2), 3)
PS C:\> $Task.Constraints = $Constraints
PS C:\> Set-AzureBatchTask -Task $Task -BatchContext $Context
```

The first command gets a task by using **Get-AzureBatchTask**, and then stores it in the $Task variable.

The next two commands modify the constraints of the task in $Task.

The final command updates the Batch service to match the local object in $Task.

## PARAMETERS

### -BatchContext
Specifies the **BatchAccountContext** instance that this cmdlet uses to interact with the Batch service.
To obtain a **BatchAccountContext** object that contains access keys for your subscription, use the Get-AzureRmBatchAccountKeys cmdlet.

```yaml
Type: BatchAccountContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Task
Specifies the **PSCloudTask** to which this cmdlet updates the Batch service.

```yaml
Type: PSCloudTask
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureBatchTask](./Get-AzureBatchTask.md)

[Get-AzureRmBatchAccountKeys](./Get-AzureRmBatchAccountKeys.md)

[New-AzureBatchTask](./New-AzureBatchTask.md)

[Remove-AzureBatchTask](./Remove-AzureBatchTask.md)

[Stop-AzureBatchTask](./Stop-AzureBatchTask.md)

[Azure Batch Cmdlets](./AzureRM.Batch.md)


