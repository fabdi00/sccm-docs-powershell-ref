---
external help file: AdminUI.PS.Sum.dll-Help.xml
Module Name: ConfigurationManager
online version:
schema: 2.0.0
---

# Remove-CMThirdPartyUpdateCatalog

## SYNOPSIS

Use this cmdlet to remove a third-party updates catalog.

## SYNTAX

### SearchByName (Default)
```
Remove-CMThirdPartyUpdateCatalog [[-Name] <String>] [-Force] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SearchByIdMandatory
```
Remove-CMThirdPartyUpdateCatalog [-Id] <String> [-Force] [-DisableWildcardHandling] [-ForceWildcardHandling]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SearchByValueMandatory
```
Remove-CMThirdPartyUpdateCatalog [-InputObject] <IResultObject> [-Force] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

Starting in version 1910, use this cmdlet to remove a third-party updates catalog.

## EXAMPLES

### Example 1: Force remove the catalog by name

This example force removes the third-party update catalog by its name.

```powershell
Remove-CMThirdPartyUpdateCatalog -Name "Contoso updates catalog" -Force
```

### Example 2: Remove the catalog as an object

This example removes the third-party update catalog as an object.

```powershell
$catalog = Get-CMThirdPartyUpdateCatalog -Name "Contoso updates catalog"
Remove-CMThirdPartyUpdateCatalog -ThirdPartyUpdateCatalog $catalog
```

## PARAMETERS

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

### -DisableWildcardHandling

This parameter treats wildcard characters as literal character values. You can't combine it with **ForceWildcardHandling**.

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

### -Force

Force remove the third-party updates catalog.

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

This parameter processes wildcard characters and may lead to unexpected behavior. It's not recommended. You can't combine it with **DisableWildcardHandling**.

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

### -Id

Specify the ID of the third-party updates catalog.

```yaml
Type: String
Parameter Sets: SearchByIdMandatory
Aliases: CatalogId

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject

Specify an object for the third-party updates catalog.

```yaml
Type: IResultObject
Parameter Sets: SearchByValueMandatory
Aliases: ThirdPartyUpdateCatalog

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name

Specify the name of the third-party updates catalog.

```yaml
Type: String
Parameter Sets: SearchByName
Aliases: CatalogName

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf

Shows what would happen if the cmdlet runs. The cmdlet doesn't run.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.ConfigurationManagement.ManagementProvider.IResultObject

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
