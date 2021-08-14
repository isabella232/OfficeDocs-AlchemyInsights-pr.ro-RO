---
title: Privileged Identity Management rol
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973241"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Permisiunile nu se acordă după activarea unui rol**

Atunci când activați un rol în Azure AD Privileged Identity Management (PIM), este posibil ca activarea să nu se propage instantaneu în toate portalurile care necesită rolul privilegiați. Uneori, chiar dacă modificarea este propagată, cache-ul web într-un portal poate avea drept consecință ca modificarea să nu aibă efect imediat.

Dacă activarea dvs. este întârziată, urmați acești pași:

1. Deconectați-vă de la portalul Azure și conectați-vă din nou. Atunci când activați un rol Azure AD sau un rol de resursă Azure, veți vedea etapele activării dvs. După ce s-au terminat toate etapele, veți vedea linkul "Deconectare". Puteți să utilizați acest link pentru a vă deconecta. Acest lucru va rezolva majoritatea cazurilor pentru întârzierea activării.
2. În PIM, verificați dacă sunteți listat ca membru al rolului.
3. Dacă activați rolul de administrator Exchange, asigurați-vă că vă deconectați și vă conectați din nou. Dacă problema persistă, deschideți un tichet de asistență și ridicați problema. Dacă vă utilizați rolul Exchange Administrator pentru a accesa Centrul de securitate și conformitate, consultați pasul următor.
4. Dacă activați un rol pentru a accesa Centrul de securitate și conformitate sau dacă activați rolul de Administrator SharePoint, vă veți experimenta o întârziere de activare de la câteva minute până la câteva ore. Aceasta este o problemă cunoscută și lucrăm în mod activ cu aceste echipe pentru a rezolva problema cât mai curând posibil.

Pentru mai multe informații, consultați:

- [Activarea rolurilor Azure AD în PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activarea rolurilor mele de resurse Azure în PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Permisiunile nu sunt eliminate după ce dezactivați un rol sau activarea rolului expiră**

Atunci când dezactivați un rol în Azure AD Privileged Identity Management sau atunci când expiră o perioadă de activare a rolului, poate exista o întârziere în care continuați să aveți acces.

Dacă dezactivarea este întârziată, urmați acești pași:

1. Dacă dezactivați rolul de administrator Exchange sau perioada de activare a rolului expiră și observați o întârziere semnificativă înainte ca permisiunile să fie eliminate, deschideți un tichet de asistență și spuneți-i inginerului de asistență să vă ajute să înfățișați un tichet cu echipa de gestionare a accesului privilegiați (PAM) din Office cu privire la această problemă.
2. Dacă perioada de activare a expirat, dar încă aveți sesiunea de browser deschisă, închideți browserul. Puteți continua să utilizați rolul până când închideți sesiunea. Aceasta este o problemă cunoscută și căutăm o remediere potențială pentru a revoca în mod activ fiecare sesiune după expirarea activării.

Dacă întârzierea dvs. este diferită de aceste două scenarii, deschideți un tichet de asistență.
