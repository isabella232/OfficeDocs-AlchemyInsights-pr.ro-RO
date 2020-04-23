---
title: 646 se configurează AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722575"
---
# <a name="configure-sync-features"></a><span data-ttu-id="769f8-102">Configurarea caracteristicilor de sincronizare</span><span class="sxs-lookup"><span data-stu-id="769f8-102">Configure sync features</span></span>

<span data-ttu-id="769f8-103">Azure AD conecta include mai multe caracteristici care sunt activate în mod implicit sau care se pot activa mai târziu.</span><span class="sxs-lookup"><span data-stu-id="769f8-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="769f8-104">Unele caracteristici necesită configurare suplimentară în anumite medii.</span><span class="sxs-lookup"><span data-stu-id="769f8-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="769f8-105">[Filtrarea](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limitelor obiectele sunt sincronizate cu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="769f8-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="769f8-106">În mod implicit, toți utilizatorii, persoanele de contact, grupurile și conturile de computer Windows 10 sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="769f8-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="769f8-107">Aveți posibilitatea să includeți sau să excludeți obiecte bazate pe domenii, o-uri sau alte atribute.</span><span class="sxs-lookup"><span data-stu-id="769f8-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="769f8-108">[Sincronizarea hash parola](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează hash parola din Active Directory local la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="769f8-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="769f8-109">Acest lucru permite gestionarea parolelor într-o singură locație, dar utilizarea aceleiași parole atât în mediul local, cât și în cel în cloud.</span><span class="sxs-lookup"><span data-stu-id="769f8-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="769f8-110">Deoarece Active Directory este sursa cu autoritate, aveți posibilitatea să utilizați propriile politici de parolă.</span><span class="sxs-lookup"><span data-stu-id="769f8-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="769f8-111">[Resetarea parolei cu autoservire (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor să își reseteze propriile parole în cloud în timp ce aplică în continuare politica locală privind parolele.</span><span class="sxs-lookup"><span data-stu-id="769f8-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="769f8-112">[Dispozitiv writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite dispozitive înregistrate în Azure AD pentru a fi scris înapoi la active directory local, astfel încât acestea să poată fi utilizate pentru acces condiționat.</span><span class="sxs-lookup"><span data-stu-id="769f8-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="769f8-113">[Împiedicați ștergerea accidentală](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată în mod implicit pentru a preveni prea multe ștergeri simultane ale obiectelor (mai mult de 500 de obiecte per sincronizare).</span><span class="sxs-lookup"><span data-stu-id="769f8-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="769f8-114">Aveți posibilitatea să modificați această setare pentru a satisface nevoile organizației.</span><span class="sxs-lookup"><span data-stu-id="769f8-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="769f8-115">[Upgrade-ul automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) este activat în mod implicit pentru instalările expres și vă ajută să vă asigurați că versiunea azure AD connect este întotdeauna curentă.</span><span class="sxs-lookup"><span data-stu-id="769f8-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
