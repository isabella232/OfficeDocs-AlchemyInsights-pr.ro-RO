---
title: Duplicarea înregistrărilor de dispozitiv în portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004166"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicarea înregistrărilor de dispozitiv în portal

Este posibil să vedeți 2 înregistrări pentru un dispozitiv în portal dacă dispozitivul nu raportează corect starea de co-gestionare pe site-ul Manager de configurare. Pentru a verifica starea de co-gestionare a unui dispozitiv, examinați coloana **Co-gestionat** pentru dispozitivul din consola Manager de configurare. Dacă coloana nu este vizibilă, puteți să o adăugați făcând clic dreapta pe orice antet de coloană și selectându-o din listă.

Valoarea co-gestionată trebuie să fie **Da**. Dacă valoarea este **Nu**, deschideți miniaplicația de client Manager de configurare pe dispozitivul clientului și verificați proprietatea **Co-gestionare** din fila General.

- Dacă valoarea este **Activat**, acest lucru indică probleme cu comunicarea de client cu Punctul de gestionare. Consultați **CCmMessaging.log** de pe dispozitiv pentru a investiga problemele potențiale de conectivitate.

- Dacă valoarea este **Dezactivat** și dispozitivul este înscris în Intune, asigurați-vă că dispozitivul a primit Politica de co-gestionare, prin revizuirea **CoManagementHandler.log** de pe dispozitiv.
