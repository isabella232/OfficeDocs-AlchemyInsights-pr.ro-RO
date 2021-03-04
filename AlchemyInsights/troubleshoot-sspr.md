---
title: Depanarea SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430217"
---
# <a name="troubleshoot-sspr"></a>Depanarea SSPR

**Am probleme cu configurarea resetării parolei**

- Dacă sunteți administrator și căutați cum să activați resetarea cu autoservire a parolei, consultați [tutorial activare SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), pentru a configura resetarea parolei pentru organizația dvs. De asemenea, este posibil să doriți să revizuiți [cerințele de licențiere](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
    - **Utilizatori Cloud Only** -orice Office 365 (O365) a plătit SKU sau Azure AD Basic
    - **Utilizatori cloud și/sau locali** -Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)
- Pentru întrebări suplimentare despre resetarea cu autoservire a parolei, consultați [secțiunea întrebări frecvente](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Primesc un mesaj de eroare**

Consultați acest articol pentru a găsi erorile comune și soluțiile lor: [Depanarea resetării parolei cu autoservire](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Am o problemă cu Politica de resetare a parolei**

- Dacă Politica de resetare a parolei nu se comportă așa cum vă așteptați sau dacă aveți întrebări despre politicile de resetare a parolei, consultați acest articol: [politicile și restricțiile prin parolă din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Politicile de resetare a parolei nu se aplică administratorilor. Microsoft impune o politică de resetare a parolei cu două porți implicite pentru orice rol de administrator Azure. Asigurați-vă că testați cu un utilizator care nu este administrator. Pentru mai multe informații despre politica de resetare a administratorului, consultați acest articol: [administratorul resetează diferențele de politică](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Nu doresc ca utilizatorii mei să înregistreze informații suplimentare de securitate pentru resetarea parolei**

Puteți să prepopulați datele (atributele de e-mail și de telefon) pentru utilizatorii care utilizează un API, PowerShell sau Azure AD Connect. Pentru a afla cum să citiți:

- [Implementarea resetării parolei fără a solicita utilizatorilor să se înregistreze](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Ce date se utilizează prin resetarea parolei](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Doresc ca utilizatorii mei să își înregistreze informațiile suplimentare de securitate pentru resetarea parolei**

1. Trebuie ca utilizatorii să își înregistreze informațiile de securitate pentru resetarea parolei cu autoservire prin direcționarea lor către [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. După ce datele sunt populate pentru utilizator (de către utilizator sau de către administrator), direcționați-vă utilizatorul către [aka.MS/SSPR](https://passwordreset.microsoftonline.com/) , pentru ca utilizatorii să poată fi împuterniciți să își reseteze propriile parole.
1. Dacă utilizatorii încă întâmpină probleme, probabil că sunt utilizatori **Sincronizați cu hash** -ul **federativ** sau cu parole. Acest lucru înseamnă că există probabil o problemă cu serviciul de writeback a parolei.