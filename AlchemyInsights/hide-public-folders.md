---
title: Ascunderea folderelor publice
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315437"
---
# <a name="hide-public-folders"></a>Ascunderea folderelor publice

**Pentru a ascunde întregul arbore de foldere publice**:

Utilizați pașii din [acest](https://aka.ms/ControlPF) articol pentru a ascunde întregul arbore de foldere publice de la selectiv sau de la toți utilizatorii.

**Pentru a ascunde un anumit folder public**:

1. Adăugarea de permisiuni pentru utilizatorii care trebuie să acceseze folderul public

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Eliminați **implicit** utilizatorul din lista de **permisiuni** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
