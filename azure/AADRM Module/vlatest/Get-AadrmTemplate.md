---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=400626
schema: 2.0.0
ms.assetid: 89C3B584-6401-46D5-BB40-5DCB41A149B4
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Get-AadrmTemplate.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Get-AadrmTemplate.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AadrmTemplate

## SYNOPSIS
Gets a list of Rights Management templates.

## SYNTAX

```
Get-AadrmTemplate [-TemplateId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmTemplate** cmdlet gets all existing or selected templates from the active Azure Rights Management tenant.
Use the *TemplateID* parameter to get a specific template.
If you do not specify the *TemplateId*, all templates are retrieved.

The cmdlet output is a list of template objects that contain all the template properties that you can use for further processing.
The output of this command displays the template GUID, name, and description in the current locale.
For additional template properties, such as usage rights and whether the template is published or archived, use the Get-AadrmTemplateProperty cmdlets.

For more information about custom templates, see Configuring custom templates for Azure Rights Managementhttps://docs.microsoft.com/rights-management/deploy-use/configure-custom-templates (https://docs.microsoft.com/rights-management/deploy-use/configure-custom-templates) on the Microsoft documentation site.

## EXAMPLES

### Example 1: Get all templates
```
PS C:\> Get-AadrmTemplate
```

This command gets all templates for your tenant, so you can get the template ID that you want to use, by identifying the template by its name and description.

### Example 2: Get a specific template
```
PS C:\> Get-AadrmTemplate -TemplateId 28168524-29c3-44f1-9e11-ea6c60bb6428
```

This command gets a specific template, specified by its template ID (GUID), so that you can confirm from its name and description that it is the template that you want to use.

## PARAMETERS

### -TemplateId
Specifies the GUID of an Rights Management template.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### TemplateID
Specifies the GUID of the template to get.

## OUTPUTS

###  
This cmdlet outputs a list comprising all templates for the tenant, or for a selected template.

If no name is defined for a template in the current locale, "No name defined in language-code" is returned as the name for that template.

If no description is defined for a template in the current locale, "No description defined in language-code" is returned as the description for that template.

## NOTES

## RELATED LINKS

[Add-AadrmTemplate](./Add-AadrmTemplate.md)

[Export-AadrmTemplate](./Export-AadrmTemplate.md)

[Import-AadrmTemplate](./Import-AadrmTemplate.md)

[Remove-AadrmTemplate](./Remove-AadrmTemplate.md)


