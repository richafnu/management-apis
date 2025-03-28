---
title: "engagement role member resource type"
description: "Represents the role management in Viva Engage which involves assigning and managing various administrative roles and corp comm role within the Viva Engage platform."
author: "richafnu"
ms.localizationpriority: medium
ms.subservice: "viva-engage"
doc_type: resourcePageType
ms.date: 03/24/2025
---

# engagement member role resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Every community is associated with a [Microsoft 365 group](../resources/group.md), but the group doesn't have the same ID as the community. For more information about managing communities in Viva Engage, see [Use the Microsoft Graph API to work with Viva Engage](../resources/engagement-api-overview.md).

Viva Engage manages role assignments where each admin has a corresponding admin role mapped in Microsoft Entra ID. These roles are assigned in the Microsoft 365 admin portal, allowing for the assignment of additional roles for management, tasks, and maintenance. For more details about admin role management in Viva Engage, see [Manage admin roles in Viva Engage | Microsoft Learn]() 

This resource is an open type that allows other properties to be passed in.

Inherits from [entity](../resources/entity.md).

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[List](../api/employeeexperience-list-userswithroles.md)|List of engagement role members|Get a list of all users who are assigned a specific role in Viva Engage.`|
|[Create](../api/employeeexperience-post-promoteuser.md)|None|Promote a user to a specific role type in Viva Engage.|
|[Delete](../api/employeeexperience-delete-demoteuser.md)|None|Demote a user from a specific role type in Viva Engage.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
| createdDataTime | DateTimeOffset | The timestamp when the role was assigned to the user. |
| displayName | String | The name of the role. The maximum length is 255 characters. |
| id | String | The unique identifier of the role. Read-only. Inherited from [entity](../resources/entity.md). |
| userOfficeId | String | The Entra/Office id of the user who has been assigned any specific role. |

## Relationships

|Relationship|Type|Description|
|:---|:---|:---|
|user|[user](../resources/user.md) collection| The users assigned a role in Viva Engage. The user directory object can be expanded to get user attributes.|

## JSON representation

The following JSON representation shows the resource type.

``` json
{
  "@odata.type": "#microsoft.graph.community",
  "createdDateTime": "DateTimeOffset",
  "displayName": "String",
  "id": "String (identifier)",
  "userId": "String"
}
```

## Related content

- [Use the Microsoft Graph API to work with Viva Engage](engagement-api-overview.md)
