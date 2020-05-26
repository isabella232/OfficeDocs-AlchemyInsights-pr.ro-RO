---
title: Blocarea descărcării la partajarea linkurilor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358034"
---
# <a name="block-download-on-sharing-links"></a>Blocarea descărcării la partajarea linkurilor

**Descărcarea blocului** este disponibilă pentru **linkurile doar pentru vizualizare** la documente Office. Când selectați această opțiune, persoanele care obțin acces la fișier prin intermediul linkului pe care l-ați creat nu vor vedea opțiunile de descărcare, imprimare sau copiere a fișierului.

Administratorii pot controla dacă setarea "block download" apare numai pentru fișierele Office sau nu prin modificarea `BlockDownloadLinksFileType` setării în cmdlet-urile [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) sau [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
