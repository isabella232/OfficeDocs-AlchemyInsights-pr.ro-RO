---
title: 646 cum se configurează AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704501"
---
# <a name="configure-sync-features"></a><span data-ttu-id="cd0dd-102">Configurarea caracteristicilor de sincronizare</span><span class="sxs-lookup"><span data-stu-id="cd0dd-102">Configure sync features</span></span>

<span data-ttu-id="cd0dd-103">Azure AD Connect include mai multe caracteristici activate în mod implicit sau pe care le puteți activa mai târziu.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="cd0dd-104">Unele caracteristici necesită o configurare suplimentară în anumite medii.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="cd0dd-105">Limite de [Filtrare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiectele sunt sincronizate cu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="cd0dd-106">În mod implicit, toți utilizatorii, persoanele de contact, grupurile și conturile de computer Windows 10 sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="cd0dd-107">Puteți să includeți sau să excludeți obiecte pe baza domeniilor, a sau a altor atribute.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="cd0dd-108">[Sincronizarea codului hash pentru parole](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează codul hash al parolei din Active Directory local la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="cd0dd-109">Acest lucru permite gestionarea parolelor într-o singură locație, dar utilizarea aceleiași parole în medii locale și în cloud.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="cd0dd-110">Deoarece Active Directory este sursa autoritară, puteți utiliza propriile politici pentru parole.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="cd0dd-111">[Resetarea parolei cu autoservire (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor să-și reseteze propriile parole în cloud în timp ce aplică în continuare Politica de parolă locală.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="cd0dd-112">[Writeback dispozitivelor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite ca dispozitivele înregistrate din Azure AD să fie scrise înapoi în Active Directory local, astfel încât să poată fi utilizate pentru acces condiționat.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="cd0dd-113">[Prevenirea ștergerii accidentale](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată în mod implicit pentru a împiedica prea multe ștergeri de obiecte simultane (mai mult de 500 de obiecte per sincronizare).</span><span class="sxs-lookup"><span data-stu-id="cd0dd-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="cd0dd-114">Puteți modifica această setare pentru a răspunde nevoilor organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="cd0dd-115">[Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) -ul automat este activat în mod implicit pentru instalările expres și vă ajută să vă asigurați că versiunea de Azure AD Connect este întotdeauna curentă.</span><span class="sxs-lookup"><span data-stu-id="cd0dd-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
