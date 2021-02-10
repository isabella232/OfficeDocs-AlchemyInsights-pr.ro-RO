---
title: Sincronizare hash parolă pentru serviciul de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177624"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="9fcc8-102">Sincronizare hash parolă pentru serviciul de domeniu</span><span class="sxs-lookup"><span data-stu-id="9fcc8-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="9fcc8-103">**Dacă instanța Azure AD DS vă solicită să activați sincronizarea codului hash pentru parole**</span><span class="sxs-lookup"><span data-stu-id="9fcc8-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="9fcc8-104">Întâlniți un scenariu în care se execută un mediu hibrid cu utilizatorii care se sincronizează dintr-un mediu Azure Active Directory (AD DS) local.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="9fcc8-105">Acest scenariu este întâlnit în ciuda faptului că aveți sincronizarea cu parola hash din AD DS local la entitatea găzduită Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="9fcc8-106">**Cauza**</span><span class="sxs-lookup"><span data-stu-id="9fcc8-106">**Cause**</span></span>

<span data-ttu-id="9fcc8-107">Acest lucru se întâmplă deoarece Azure AD Connect în mod implicit nu sincronizează noile hash-uri de tehnologie LAN Manager (NTLM) și Kerberos password care sunt necesare pentru Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="9fcc8-108">**Soluție**</span><span class="sxs-lookup"><span data-stu-id="9fcc8-108">**Workaround**</span></span> 

<span data-ttu-id="9fcc8-109">Trebuie să configurați Azure AD Connect pentru a sincroniza acele parole hash necesare pentru autentificarea NTLM și Kerberos.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="9fcc8-110">După ce Azure AD Connect este configurat, un eveniment local de creare a unui cont sau de modificare a parolei, de asemenea, sincronizează hash-ul de parolă moștenit la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="9fcc8-111">Vă rugăm să consultați [aici](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) pentru mai multe informații despre aceasta și pentru instrucțiuni despre cum să activați sincronizarea parolelor în medii hibride AZURE AD DS.</span><span class="sxs-lookup"><span data-stu-id="9fcc8-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>