---
title: Atribuirea grupurilor la rolul Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036252"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Atribuirea grupurilor la rolul Azure AD

Pentru a atribui un grup Azure AD cu sursă de autoritate în Azure AD la un rol Azure AD, efectuați pașii următori:

1. Creați un grup nou - Pentru a crea un grup nou:

    a. Conectați-vă la centrul de administrare Azure AD cu **permisiuni de administrator cu rol de privilegiați** sau de **administrator** global.
    b. Selectați **Azure Active Directory > Grupuri > Toate grupurile > Grup nou.**
    c. Creați grupul.

2. Atribuiți rolul grupului în timpul creării grupului sau după crearea grupului.

    a. Pentru a atribui un rol grupului în momentul creării grupului, comutați butonul De comutare Rolurile **Azure AD** pot fi atribuite grupului și creați grupul.
    b. Pentru a atribui un rol grupului după ce  a fost creat, navigați la fila Roluri atribuite pentru grupul nou creat și atribuiți rolul grupului.  

**Gestionarea apartenenței unui grup care este atribuit rolului Azure AD**

Pentru a împiedica cota privilegiilor, în mod implicit, doar administratorii cu roluri privilegiați și administratorii globali pot modifica apartenența unui grup atribuit unui rol. Însă pot alege să atribuie un proprietar pentru un astfel de grup și să delege această activitate.

Pentru mai multe detalii despre atribuirea grupurilor cloud rolurilor Azure AD, consultați Atribuirea [rolurilor AD grupului în cloud.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Pentru mai multe detalii despre rolurile de depanare atribuite grupurilor în cloud, consultați [Depanarea rolurilor atribuite grupurilor în cloud.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





