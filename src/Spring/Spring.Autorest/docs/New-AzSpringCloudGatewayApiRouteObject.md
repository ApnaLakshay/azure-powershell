---
external help file:
Module Name: Az.SpringApps
online version: https://learn.microsoft.com/powershell/module/Az.SpringApps/new-azspringcloudgatewayapirouteobject
schema: 2.0.0
---

# New-AzSpringCloudGatewayApiRouteObject

## SYNOPSIS
Create an in-memory object for GatewayApiRoute.

## SYNTAX

```
New-AzSpringCloudGatewayApiRouteObject [-Description <String>] [-Filter <String[]>] [-Order <Int32>]
 [-Predicate <String[]>] [-SsoEnabled <Boolean>] [-Tag <String[]>] [-Title <String>] [-TokenRelay <Boolean>]
 [-Uri <String>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for GatewayApiRoute.

## EXAMPLES

### Example 1: Create an in-memory object for GatewayApiRoute.
```powershell
New-AzSpringCloudGatewayApiRouteObject -Title "myApp route config" -SsoEnabled $true -Filter "StripPrefix=2","RateLimit=1,1s" -Predicate "Path=/api5/customer/**"
```

```output
Description :
Filter      : {StripPrefix=2, RateLimit=1,1s}
Order       :
Predicate   : {Path=/api5/customer/**}
SsoEnabled  : True
Tag         :
Title       : myApp route config
TokenRelay  :
Uri         :
```

Create an in-memory object for GatewayApiRoute.

## PARAMETERS

### -Description
A description, will be applied to methods in the generated OpenAPI documentation.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
To modify the request before sending it to the target endpoint, or the received response.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Order
Route processing order.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Predicate
A number of conditions to evaluate a route for each request.
Each predicate may be evaluated against request headers and parameter values.
All of the predicates associated with a route must evaluate to true for the route to be matched to the request.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SsoEnabled
Enable sso validation.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tag
Classification tags, will be applied to methods in the generated OpenAPI documentation.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
A title, will be applied to methods in the generated OpenAPI documentation.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TokenRelay
Pass currently-authenticated user's identity token to application service, default is 'false'.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Uri
Full uri, will override ppName.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

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

### Microsoft.Azure.PowerShell.Cmdlets.SpringApps.Models.GatewayApiRoute

## NOTES

## RELATED LINKS

