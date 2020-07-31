---
external help file: AdminUI.PS.HS.dll-Help.xml
Module Name: ConfigurationManager
online version:
schema: 2.0.0
---

# Add-CMPassiveSite

## SYNOPSIS
Use this cmdlet to add a site server in passive mode.

## SYNTAX

### AddByInputObjectMandatory (Default)
```
Add-CMPassiveSite -InputObject <IResultObject> -InstallDirectory <String>
 -SourceFilePathOption <PassiveSiteSourceFileType> [-LocalSourceDirectory <String>]
 [-NetworkSourceDirectory <String>] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### AddBySiteCodeMandatory
```
Add-CMPassiveSite -SiteCode <String> -SiteSystemServerName <String> -InstallDirectory <String>
 -SourceFilePathOption <PassiveSiteSourceFileType> [-LocalSourceDirectory <String>]
 [-NetworkSourceDirectory <String>] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Starting in version 2002, use this cmdlet to add a site server in passive mode.

## EXAMPLES

### Example 1

```powershell
Add-CMPassiveSite -InputObject $SiteSystem -InstallDirectory $InstallPath -SourceFilePathOption CopySourceFileFromActiveSite
```

### Example 2

```powershell
Add-CMPassiveSite -SiteCode $SiteCode -SiteSystemServerName $SiteSystemServerName -InstallDirectory $InstallPath -SourceFilePathOption UseLocalSourceDirectory -LocalSourceDirectory $LocalSourcePath
```

## PARAMETERS

### -DisableWildcardHandling
{{ Fill DisableWildcardHandling Description }}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
{{ Fill ForceWildcardHandling Description }}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{ Fill InputObject Description }}

```yaml
Type: IResultObject
Parameter Sets: AddByInputObjectMandatory
Aliases: SiteSystemServer

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InstallDirectory
{{ Fill InstallDirectory Description }}

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalSourceDirectory
{{ Fill LocalSourceDirectory Description }}

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

### -NetworkSourceDirectory
{{ Fill NetworkSourceDirectory Description }}

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

### -SiteCode
{{ Fill SiteCode Description }}

```yaml
Type: String
Parameter Sets: AddBySiteCodeMandatory
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteSystemServerName
{{ Fill SiteSystemServerName Description }}

```yaml
Type: String
Parameter Sets: AddBySiteCodeMandatory
Aliases: Name, ServerName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceFilePathOption
{{ Fill SourceFilePathOption Description }}

```yaml
Type: PassiveSiteSourceFileType
Parameter Sets: (All)
Aliases:
Accepted values: CopySourceFileFromActiveSite, UseLocalSourceDirectory, UseNetworkSourceDirectory

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_commonparameters?view=powershell-7).

## INPUTS

### Microsoft.ConfigurationManagement.ManagementProvider.IResultObject

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS

[Site server high availability](https://docs.microsoft.com/mem/configmgr/core/servers/deploy/configure/site-server-high-availability)