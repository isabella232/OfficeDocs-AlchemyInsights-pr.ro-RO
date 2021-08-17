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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038970"
---
# <a name="troubleshoot-sspr"></a>Depanarea SSPR

**Am probleme cu configurarea resetării parolei**

- Dacă sunteți administrator și căutați cum să activați resetarea parolei cu autoservre, consultați [Tutorial activareA SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)pentru a configura resetarea parolei pentru organizația dvs. De asemenea, este posibil să doriți să revizuiți [cerințele de licențiere.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
    - **Doar utilizatorii din** cloud - orice SKU cu plată Office 365 (O365) sau Azure AD Basic
    - **Utilizatori în cloud și/sau** locali - Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure Productive Enterprise (SPE)
- Pentru întrebări suplimentare despre resetarea parolei cu autoservre, consultați [Întrebările frecvente](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Primesc un mesaj de eroare**

Consultați acest articol pentru a găsi erori comune și soluțiile lor: Depanarea [resetării parolei cu autoservre](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Am o problemă cu politica mea de resetare a parolei**

- Dacă politica de resetare a parolei nu are un comportament așa cum vă așteptați sau dacă aveți întrebări despre politicile de resetare a parolei, consultați acest articol: Politicile privind parolele și restricțiile din [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Politicile de resetare a parolei nu se aplică administratorilor. Microsoft impune o politică puternică de resetare a parolei de două porți pentru orice rol de administrator Azure. Asigurați-vă că testați cu un utilizator care nu este administrator. Pentru mai multe informații despre politica de resetare a administratorilor, consultați acest articol: Diferențele între [politicile de resetare a administratorilor.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nu doresc ca utilizatorii mei să înregistreze informații de securitate suplimentare pentru resetarea parolei**

Puteți prepopula datele (e-mailul și atributele telefonului) pentru utilizatorii dvs. utilizând un raport API, PowerShell sau Azure AD Conectare. Pentru a afla cum să citiți:

- [Implementarea resetării parolei fără a fi necesar ca utilizatorii să se înregistreze](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Ce date sunt utilizate pentru resetarea parolei](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Doresc ca utilizatorii mei să-și înregistreze informațiile de securitate suplimentare pentru resetarea parolei**

1. Spuneți-le utilizatorilor să-și înregistreze informațiile de securitate pentru resetarea cu autoservire a [parolei, direcționându-i aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. După popularea datelor pentru utilizator (de către utilizator sau de administrator), direcționați utilizatorul către [aka.ms/sspr](https://passwordreset.microsoftonline.com/) astfel încât utilizatorii să poată fi admiți să își reseteze parolele.
1. Dacă utilizatorii încă întâmpină probleme, cel mai probabil sunt utilizatori **federativi** sau **cu sincronizarea parolelor.** Acest lucru înseamnă că este probabil o problemă cu serviciul WriteBack parole.