---
title: Configurarea serviciului de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885690"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nu reușiți să activați AAD-DS sau implementarea nu reușește

Pentru a rezolva problema serviciului de domeniu Azure AD (AAD-DS) care nu este activat sau nu este implementat, efectuați pașii următori:

1. Dacă utilizați o rețea virtuală deja existentă, Verificați-vă NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în AAD-DS în portal https://aka.ms/aadds-networking .
2. Verificați dacă mesajul de eroare este răspuns în acest ghid de depanare disponibil în  https://aka.ms/aadds-troubleshoot-enable .
3. Încercați să implementați servicii de domeniu Azure AD într-o rețea virtuală nouă.
4. Urmați ghidul introductiv despre cum să implementați AAD-DS: [crearea și configurarea serviciilor de domeniu AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Dacă întâmpinați probleme cu implementarea serviciilor de domeniu Azure AD, consultați [Depanarea serviciilor de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pentru a rezolva erorile comune, pentru a vă ajuta să lucrați din nou. 

**Nu se poate dezactiva AAD-DS**

AAD-DS nu poate fi în pauză. Dacă doriți să opriți utilizarea domeniului gestionat, acesta trebuie șters.
Pentru a șterge domeniul gestionat, consultați [ștergerea serviciului de domeniu AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



