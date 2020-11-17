---
title: Rol privilegiat de gestionare a identității
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089154"
---
# <a name="privileged-identity-managementpim-role"></a>Rolul de gestionare a identității privilegiat (PIM)

**Permisiunile nu se acordă după activarea unui rol**

Atunci când activați un rol în Azure AD privilegiat Identity Management (PIM), activarea poate să nu se propage instantaneu la toate portaluri care necesită rolul privilegiat. Uneori, chiar dacă modificarea este propagată, memorarea în cache Web într-un portal poate avea ca rezultat modificarea care nu intră în vigoare imediat.

Dacă activarea este întârziată, urmați acești pași:

1. Deconectați-vă de la portalul Azure, apoi conectați-vă din nou. Atunci când activați un rol Azure AD sau un rol de resurse Azure, veți vedea etapele de activare. După ce se termină toate etapele, veți vedea un link "deconectare". Puteți utiliza acest link pentru a vă deconecta. Acest lucru va rezolva majoritatea cazurilor pentru întârzierea activării.
2. În PIM, asigurați-vă că sunteți listat ca membru al rolului.
3. Dacă activați rolul de administrator Exchange, asigurați-vă că vă deconectați și vă conectați din nou. Dacă problema persistă, deschideți un tichet de asistență și creșteți-l ca problemă. Dacă utilizați rolul de administrator Exchange pentru a accesa centrul de securitate și conformitate, consultați Pasul următor.
4. Dacă activați un rol pentru a accesa centrul de securitate și conformitate sau dacă activați rolul de administrator SharePoint, veți avea câteva întârzieri de activare de la câteva minute până la câteva ore. Aceasta este o problemă cunoscută și lucrăm în mod activ cu aceste echipe pentru a rezolva această problemă cât mai curând posibil.

Pentru mai multe informații, consultați:

- [Activarea rolurilor de publicitate Azure în PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activarea rolurilor de resurse Azure în PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Permisiunile nu sunt eliminate după ce dezactivarea unui rol sau activarea rolului expiră**

Atunci când dezactivați un rol în managementul de identitate privilegiat din Azure AD sau când expiră o perioadă de activare a rolului, poate exista o întârziere în care continuați să aveți acces.

Dacă dezactivarea este întârziată, urmați acești pași:

1. Dacă deactivați rolul de administrator Exchange sau perioada de activare a rolului expiră și observați o întârziere semnificativă înainte ca permisiunile să fie eliminate, deschideți un tichet de asistență și spuneți-i inginerului de asistență să vă ajute să faceți un bilet cu echipa de gestionare a accesului privilegiat (PAM) în Office despre această problemă.
2. Dacă perioada de activare a expirat, dar încă aveți sesiunea de browser deschisă, închideți browserul. Puteți continua să utilizați rolul până când închideți acea sesiune. Aceasta este o problemă cunoscută și ne uităm la o remediere potențială pentru a revoca în mod activ fiecare sesiune după ce activarea a expirat.

Dacă întârzierea dumneavoastră este diferită de aceste două scenarii, vă rugăm să deschideți un tichet de asistență.
