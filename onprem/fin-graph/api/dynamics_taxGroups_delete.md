---
title: Delete taxGroups | Microsoft Docs
description: Deletes a tax group object in Dynamics 365 Business Central. 
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/08/2018
ms.author: solsen
---

# Delete taxGroups
Delete a tax group object from Dynamics 365 Business Central.

## HTTP request
```
DELETE /businesscentral/companies({id})/taxGroups({id})
```

## Request headers
|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |
|If-Match       |Required. When this request header is included and the eTag provided does not match the current tag on the **taxGroups**, the **taxGroups** will not be updated. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns ```204,No Content``` response code. It does not return anything in the response body.

## Example

**Request**

Here is an example of the request.

```json
DELETE https://api.businesscentral.dynamics.com/v1.0/api/beta/companies({id})/taxGroups({id})
```

**Response** 

Here is an example of the response. 

```json
HTTP/1.1 204 No Content
```

## See Also
[Graph Reference](../api/dynamics_graph_reference.md)  
[Working with [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] in Microsoft Graph](../resources/dynamics_overview.md)  
[Enabling the APIs for Microsoft Dynamics NAV](../enabling-apis-for-dynamics-nav.md)  
[Endpoints for the APIs](../endpoints-apis-for-dynamics.md)  
[Error Codes](../dynamics_error_codes.md)  
[Tax groups](../resources/dynamics_taxgroups.md)  
[Get tax groups](../api/dynamics_taxgroups_get.md)  
[Create tax groups](../api/dynamics_create_taxgroups.md)  
[Update tax groups](../api/dynamics_taxgroups_update.md)  