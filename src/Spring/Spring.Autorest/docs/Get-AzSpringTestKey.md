---
external help file:
Module Name: Az.SpringApps
online version: https://learn.microsoft.com/powershell/module/az.springapps/get-azspringtestkey
schema: 2.0.0
---

# Get-AzSpringTestKey

## SYNOPSIS
List test keys for a Service.

## SYNTAX

```
Get-AzSpringTestKey -Name <String> -ResourceGroupName <String> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
List test keys for a Service.

## EXAMPLES

### Example 1: List test keys for a Service.
```powershell
Get-AzSpringTestKey -Name azps-spring-01 -ResourceGroupName azps_test_group_spring
```

```output
Enabled               : True
PrimaryKey            : AL4W969BM5bfDRyXsa3WXtxpQHr5dL6f3RGnq2Xf6BZ3VFA4WXs7scSklzNAudKE
PrimaryTestEndpoint   : https://primary:AL4W969BM5bfDRyXsa3WXtxpQHr5dL6f3RGnq2Xf6BZ3VFA4WXs7scSklzNAudKE@azps-spring-01.test.azuremicroservices.io
SecondaryKey          : HiagYRIgAPJpFkOSxRFDjXzVDQ6d4QBWRMW89WCgCQKCMPvaYEhK4VThpKesfzYT
SecondaryTestEndpoint : https://secondary:HiagYRIgAPJpFkOSxRFDjXzVDQ6d4QBWRMW89WCgCQKCMPvaYEhK4VThpKesfzYT@azps-spring-01.test.azuremicroservices.io
```

List test keys for a Service.

### Example 2: List test keys for a Service.
```powershell
Disable-AzSpringTestEndpoint -ResourceGroupName azps_test_group_spring -Name azps-spring-01
Get-AzSpringTestKey -Name azps-spring-01 -ResourceGroupName azps_test_group_spring
```

```output
Enabled               : False
PrimaryKey            :
PrimaryTestEndpoint   :
SecondaryKey          :
SecondaryTestEndpoint :
```

List test keys for a Service.

## PARAMETERS

### -DefaultProfile
The DefaultProfile parameter is not functional.
Use the SubscriptionId parameter when available if executing the cmdlet against a different subscription.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The name of the Service resource.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group that contains the resource.
You can obtain this value from the Azure Resource Manager API or the portal.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
Gets subscription ID which uniquely identify the Microsoft Azure subscription.
The subscription ID forms part of the URI for every service call.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
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
Type: System.Management.Automation.SwitchParameter
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

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.SpringApps.Models.ITestKeys

## NOTES

## RELATED LINKS

