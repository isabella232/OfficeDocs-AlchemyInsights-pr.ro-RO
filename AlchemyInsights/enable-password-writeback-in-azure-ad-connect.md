---
title: Activați Rescriere parole în Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118216"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Activați Rescriere parole în Azure AD Connect

Pentru a activa resetarea opțiunii Rescriere parole, mai întâi activați opțiunea Rescriere parole în Azure AD Connect. Din serverul dvs. Azure AD Connect, completați următorii pași:

1. Conectați-vă la serverul dvs. Azure AD Connect și demarați expertul de configurare **Azure AD Connect**.
2. Pe pagina **Bun venit**, faceți clic pe **Configurare**.
3. Pe pagina **Activități suplimentare**, selectați **Particularizare opțiuni de sincronizare**, și apoi faceți clic pe **Următorul**.
4. Pe pagina **Conectare la Azure AD**, introduceți o acreditare administrator global pentru locatarul Azure și apoi faceți clic pe **Următorul**.
5. În directoarele **Conectare** și paginile de filtrare **Domain/OU** faceți clic pe **Următorul**.
6. Pe pagina **Caracteristici opționale**, selectați caseta de lângă **Rescriere parole** și faceți clic pe **Următorul**.
7. Pe pagina **Gata de configurat**, faceți clic pe **Configurare** și așteptați terminarea procesului.
8. Atunci când vedeți că s-a terminat configurarea, faceți clic pe **Ieșire**.

Cu Rescrierea parolei activată în Azure AD Connect, configurați Azure AD SSPR pentru rescrierea parolei.  Pentru a activa rescrierea parolei în SSPR, completați următorii pași:

1. Conectați-vă la portalul Azure utilizând un cont de administrator global.
2. Căutați și selectați **Azure Active Directory**, faceți clic pe **Resetare parolă**, apoi faceți clic pe **Integrare locală**.
3. Setați opțiunea **Rescriere parole pentru directorul local?** la **Da**.
4. Setați opțiunea **Permiteți utilizatorilor să deblocheze conturile fără a-și reseta parolele?** la **Da**.
5. Atunci când sunteți pregătit, faceți clic pe **Salvare**.

Pentru mai multe informații, vedeți [Activarea rescrierii parolelor în Azure Active Directory într-un domeniu local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Atunci când un administrator resetează parola unui utilizator în portalul Azure, dacă acel utilizator este federativ sau hash-ul parolei este sincronizat, parola este scrisă din nou la local. Această funcționalitate necesită licență Azure Premium (P1 sau P2) și nu este acceptată momentan în portalul de administrare Office.
