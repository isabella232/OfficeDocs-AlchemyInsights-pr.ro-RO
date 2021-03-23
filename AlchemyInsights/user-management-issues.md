---
title: Probleme de gestionare a utilizatorilor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037506"
---
# <a name="user-management-issues"></a>Probleme de gestionare a utilizatorilor

**Ce se întâmplă cu utilizatorii desemnați actuali la aplicație dacă dezactivez proprietatea "atribuire utilizator necesară" (setați această proprietate la nu)?**

Dezactivarea atribuirii de **utilizator necesară** nu afectează utilizatorii desemnați în prezent. Dezactivarea acestei proprietăți va permite tuturor utilizatorilor să acceseze aplicația. Toți utilizatorii enumerați și acei utilizatori atribuiți grupurilor din aplicație vor fi în continuare Validi.

- Pentru a restricționa aplicația la un anumit set de utilizatori, consultați- [restricționarea aplicației AZURE ad la un set de utilizatori-platforma de identitate Microsoft | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Pentru a atribui utilizatori și grupuri, aplicațiilor de întreprindere din Azure Active Directory (Azure AD), fie din cadrul portalului Azure, fie utilizând PowerShell, consultați [gestionarea atribuirii de utilizator pentru o aplicație din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Pentru a delega permisiunile de creare și gestionare a aplicațiilor, consultați [delegare permisiuni de administrator de gestionare a aplicațiilor-AZURE AD | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ascunderea anumitor aplicații de întreprindere de la utilizatori** -utilizați următorii pași pentru a ascunde toate aplicațiile Microsoft 365 din panoul **aplicațiile mele** . Aplicațiile vor fi în continuare vizibile în portalul Office 365.

 1. Conectați-vă la portalul Azure ca administrator global pentru directorul dvs. 
 2. Selectați **Azure Active Directory**. 
 3. Selectați **utilizatori**. 
 4. Selectați **Setări utilizator**. 
 5. Sub **aplicații Enterprise**, faceți clic pe **Gestionați modul în care utilizatorii finali lansează și vizualizează aplicațiile**. 
 6. Pentru ca **utilizatorii să poată vedea doar aplicațiile office 365 în portalul office 365**, faceți clic pe **Da**. 
 7. Faceți clic pe **Salvare**. 
 8. Pentru mai multe detalii, consultați [ascunderea unei aplicații de întreprindere din experiența utilizatorului în AZURE AD | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Dacă oferiți o aplicație software ca serviciu (SaaS) la mai multe organizații, puteți configura aplicația pentru a accepta conectarea de la orice entitate găzduită Azure Active Directory (Azure AD). Această configurație se numește "efectuarea aplicației multi-entitate găzduită". Utilizatorii din orice entitate găzduită Azure AD vor putea să se conecteze la aplicație după ce consimte să își utilizeze contul cu aplicația dvs. Pentru mai multe informații, consultați [generarea aplicațiilor care se conectează la utilizatorii AZURE AD-platforma de identitate Microsoft | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Cum poate un utilizator final să acceseze aplicația după ce acesta este atribuit aplicației?**

Fiecare aplicație din aplicația Enterprise Blade are un link pentru ca utilizatorii finali să aibă acces. De asemenea, utilizatorii pot accesa aplicația prin portalul **aplicațiile mele** într-un mod simplu.

- **Doriți să știți ce aplicații și tipuri de aplicații sunt utilizate de utilizatori?**

Puteți descărca rapoarte de conectare pentru ultimele 30 de zile de la **portal.azure.com > Azure Active directory> Signins> descărcarea rapoartelor**.

- Aflați cum să [acordați consimțământul administratorului pentru entități găzduite la o aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) și să [configurați modul în care utilizatorii finali sunt de acord cu aplicațiile](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Înțelegeți [cum funcționează consimțământul](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) și [Gestionați consimțământul pentru aplicații](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


