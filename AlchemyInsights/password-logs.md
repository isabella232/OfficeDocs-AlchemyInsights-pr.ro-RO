---
title: Jurnale de parole
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527179"
---
# <a name="password-logs"></a>Jurnale de parole

**Am probleme cu accesarea jurnalelor de audit de resetare a parolei**

Pentru a depana problemele cu privire la accesul la jurnalele de audit de resetare a parolei, efectuați următorul pas:

Asigurați-vă că sunteți autorizat să vizualizați jurnalele de auditare. 

Sunt autorizate doar următoarele roluri:
 - Administrator global
 - Administrator de securitate
 - Cititor de securitate

**Doresc să văd toate evenimentele de audit de resetare a parolei din momentul în care am implementat inițial**

Până la 120.000 de resetare a parolei/evenimente de înregistrare sunt stocate în rapoartele din ultimele 30 de zile. Această limită maximă se aplică la interfața de utilizator atunci când descărcați CSV. evenimentele 1.000.000 sunt disponibile prin PowerShell.
Pentru mai multe informații, consultați linkurile de mai jos:

- [Evenimente de resetare a parolei cu autoservire din API-ul de rapoarte și evenimente Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cum se descarcă rapid evenimentele de înregistrare a resetării parolelor cu PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Doresc să înțeleg mai multe despre capacitățile de raportare a resetării parolei**

Verificați cine înregistrează sau reinițializează parolele cu jurnalele de audit Azure AD reinițializare a parolelor în portalul Azure, sub **utilizatori și grupuri**.
Pentru mai multe informații, consultați următoarele linkuri:

- [Prezentare generală a rapoartelor de resetare a parolei](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cum se vizualizează rapoartele de resetare a parolei în portalul Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Evenimente de resetare a parolei cu autoservire din API-ul de rapoarte și evenimente Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cum se descarcă rapid evenimentele de înregistrare a resetării parolelor cu PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


