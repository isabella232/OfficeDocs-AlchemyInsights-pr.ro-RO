---
title: Probleme cu Proprietarul înregistrării aplicațiilor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951145"
---
# <a name="app-registration-owner-issues"></a>Probleme cu Proprietarul înregistrării aplicațiilor

În cele ce urmează, metodele disponibile pentru adăugarea de directori ca proprietari pentru înregistrările aplicațiilor:

- Utilizarea Modulului Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referință: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Utilizarea Azure CLI - `az ad app owner add`

    Referință: [proprietar al aplicației az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Utilizarea MS Graph -

    Referință: [Adăugare proprietar - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Utilizarea Portalului Azure AD - Navigați [la portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Înregistrarea aplicațiilor > Selectați-vă aplicația > proprietarii > Adăugați proprietari

**Nu puteți vizualiza aplicația blade pentru înregistrările aplicațiilor chiar dacă sunteți proprietarul aplicației?**

Proprietarul unei aplicații nu este un rol administrativ. În cazul în care setarea Restricționați accesul la portalul de administrare [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) este activată, doar administratorul va putea vizualiza aplicațiile în portalul de înregistrare a aplicațiilor. Pentru ca un proprietar să poată vedea aplicațiile, dezactivați această setare (Setați la NU) sau atribuiți rolul de administrator proprietarului doar pentru aplicația specifică. Cu toate acestea, veți solicita o licență Azure AD Premium P2 și veți activa [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
