---
title: 646 cum la spre configure AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541597"
---
# <a name="configure-sync-features"></a><span data-ttu-id="39942-102">Configurați sincronizare caracteristici</span><span class="sxs-lookup"><span data-stu-id="39942-102">Configure sync features</span></span>

<span data-ttu-id="39942-103">Azur AD Connect include mai multe caracteristici care sunt activate în mod implicit, sau puteţi activa mai tarziu.</span><span class="sxs-lookup"><span data-stu-id="39942-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="39942-104">Unele funcții necesită configurare suplimentare în anumite medii.</span><span class="sxs-lookup"><span data-stu-id="39942-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="39942-105">[Filtrarea](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limitele obiectele sunt sincronizate cu Azur AD.</span><span class="sxs-lookup"><span data-stu-id="39942-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="39942-106">Mod implicit, tuturor utilizatorilor, contacte, grupuri, şi Windows 10 calculator conturi sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="39942-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="39942-107">Pot include sau exclude obiecte bazate pe domenii, Pension sau alte atribute.</span><span class="sxs-lookup"><span data-stu-id="39942-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="39942-108">[Sincronizare de hash parola](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează hash parola din Active Directory local azuriu AD.</span><span class="sxs-lookup"><span data-stu-id="39942-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="39942-109">Acest lucru permite de gestionare a parolei într-o singură locaţie, dar utilizează aceeaşi parolă în ambele locală şi nor medii.</span><span class="sxs-lookup"><span data-stu-id="39942-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="39942-110">Pentru Active Directory este sursă de autoritate, puteţi utiliza propriile politici de parola.</span><span class="sxs-lookup"><span data-stu-id="39942-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="39942-111">[(SSPR) de resetare a parolei autoservire](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor pentru a reseta parolele în nor în timp ce încă aplică politica de parola dumneavoastră local.</span><span class="sxs-lookup"><span data-stu-id="39942-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="39942-112">[Dispozitivul writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite dispozitivelor înregistraţi în Azur Anunţul să fi scris înapoi în Active Directory local astfel încât ele pot fi folosite pentru acces condiționat.</span><span class="sxs-lookup"><span data-stu-id="39942-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="39942-113">[Prevenirea accidental şterge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată implicit pentru a preveni prea multe obiecte simultan ştergeri (peste 500 de obiecte pe sincronizare).</span><span class="sxs-lookup"><span data-stu-id="39942-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="39942-114">Puteţi modifica această setare pentru a satisface nevoile dvs.</span><span class="sxs-lookup"><span data-stu-id="39942-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="39942-115">[Actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) este activată implicit pentru instalatii expres şi ajută la asigurarea versiunea de AD Azure Connect este întotdeauna curent.</span><span class="sxs-lookup"><span data-stu-id="39942-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
