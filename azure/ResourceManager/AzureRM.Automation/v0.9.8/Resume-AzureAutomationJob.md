---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version: .\Get-AzureAutomationJob.md
schema: 2.0.0
ms.assetid: 2266E168-7A9E-4D70-AA3A-69FF18FF1DD1
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v0.9.8/Resume-AzureAutomationJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v0.9.8/Resume-AzureAutomationJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Resume-AzureAutomationJob

## SYNOPSIS
Resumes a suspended Automation job.

## SYNTAX

```
Resume-AzureAutomationJob [-Id] <Guid> [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Resume-AzureAutomationJob** cmdlet resumes a suspended Azure Automation job.
Specify the suspended job.

To suspend a job, use the Suspend-AzureAutomationJob cmdlet.

## EXAMPLES

### Example 1: Resume a suspended job
```
PS C:\>Resume-AzureAutomationJob -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b64 -ResourceGroupName "ResourceGroup01"
```

This command resumes the job that has the specified ID.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Automation account in which this cmdlet resume a job.

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

### -Id
Specifies the ID of a job that this cmdlet resumes.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: JobId

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

### -ResourceGroupName
The resource group name.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureAutomationJob](./Get-AzureAutomationJob.md)

[Get-AzureAutomationJobOutput](./Get-AzureAutomationJobOutput.md)

[Stop-AzureAutomationJob](./Stop-AzureAutomationJob.md)

[Suspend-AzureAutomationJob](./Suspend-AzureAutomationJob.md)


