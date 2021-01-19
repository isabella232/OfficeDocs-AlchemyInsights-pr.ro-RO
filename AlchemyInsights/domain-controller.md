---
title: Controler de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901311"
---
# <a name="domain-controller"></a>Controler de domeniu

**Nu reușiți să activați AAD-DS sau implementarea nu reușește**

Pentru a rezolva problema serviciului de domeniu Azure AD (AAD-DS) care nu este activat sau nu este implementat, efectuați pașii următori:

1. Dacă utilizați o rețea virtuală deja existentă, Verificați-vă NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în AAD-DS în portal https://aka.ms/aadds-networking .
2. Verificați dacă mesajul de eroare este răspuns în acest ghid de depanare disponibil în  https://aka.ms/aadds-troubleshoot-enable .
3. Încercați să implementați servicii de domeniu Azure AD într-o rețea virtuală nouă.
4. Urmați ghidul introductiv despre cum să implementați AAD-DS, disponibil la [tutorial pentru a crea servicii de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Dacă întâmpinați probleme cu implementarea serviciilor de domeniu Azure AD, consultați [Depanarea serviciilor de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pentru a rezolva erorile comune, pentru a vă ajuta să lucrați din nou. 

**Nu se poate dezactiva AAD-DS**

AAD-DS nu poate fi în pauză. Dacă doriți să opriți utilizarea domeniului gestionat, acesta trebuie șters.

Dacă întâmpinați probleme, pentru a rezolva mesaje de eroare comune și pentru pașii de depanare asociați, pentru a vă ajuta să începeți lucrul, consultați [Depanarea serviciilor de domeniu Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
