---
title: "engagement role resource type"
description: "Represents the role management in Viva Engage which involves assigning and managing various administrative roles and corp comm role within the Viva Engage platform."
author: "richafnu"
ms.localizationpriority: medium
ms.subservice: "viva-engage"
doc_type: resourcePageType
ms.date: 03/24/2025
---

# engagement role resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Viva Engage manages role assignments where each admin has a corresponding admin role mapped in Microsoft Entra ID. These roles are assigned in the Microsoft 365 admin portal, allowing for the assignment of additional roles for management, tasks, and maintenance. For more details about admin role management in Viva Engage, see [Manage admin roles in Viva Engage | Microsoft Learn]() 

Inherits from [entity](../resources/entity.md).

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[List](../api/employeeexperience-get-roles.md)|List of engagement role |Get a static list of role types available in Viva Engage.|
|[List](../api/employeeexperience-get-assignedtoauser.md)|List of engagement role|List all roles assigned to a user in Viva Engage.|
|[List](../api/employeeexperience-post-promoteuser.md)|List of engagement role|List roles assigned to the logged in user.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
| displayName | String | The name of the role. The maximum length is 255 characters. |
| id | String | The unique identifier of the role. Read-only. Inherited from [entity](../resources/entity.md). |

## JSON representation

The following JSON representation shows the resource type.

``` json
{
  "@odata.type": "#microsoft.graph.community",
  "displayName": "String",
  "id": "String (identifier)"
}
```

## Related content

- [Use the Microsoft Graph API to work with Viva Engage](engagement-api-overview.md)
