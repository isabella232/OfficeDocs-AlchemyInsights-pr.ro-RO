---
title: Problemă cu AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483117"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="ce93b-102">Problemă cu AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="ce93b-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="ce93b-103">Asigurați-vă că sunteți autorizat să efectuați operațiunea.</span><span class="sxs-lookup"><span data-stu-id="ce93b-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="ce93b-104">Administratorii globali au acces în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="ce93b-104">Global Admins have access by default.</span></span> <span data-ttu-id="ce93b-105">În plus, puteți utiliza [controlul Access bazat pe roluri](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) pentru a delega permisiunea de înregistrare la colaborator.</span><span class="sxs-lookup"><span data-stu-id="ce93b-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="ce93b-106">Asigurați-vă că punctele finale necesare sunt activate și nu sunt blocate din cauza firewallului.</span><span class="sxs-lookup"><span data-stu-id="ce93b-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="ce93b-107">Pentru detalii, consultați [cerințe](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="ce93b-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="ce93b-108">Înregistrarea poate să nu reușească din cauza comunicării de ieșire supusă inspecției SSL de către stratul de rețea.</span><span class="sxs-lookup"><span data-stu-id="ce93b-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="ce93b-109">Asigurați-vă că ați verificat setările de notificare pentru Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="ce93b-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="ce93b-110">Vă rugăm să vă revizuiți setarea.</span><span class="sxs-lookup"><span data-stu-id="ce93b-110">Please review your setting.</span></span> <span data-ttu-id="ce93b-111">Acest [Ghid](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vă poate ajuta să înțelegeți cum să configurați setările de notificare pentru notificările de sănătate Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ce93b-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="ce93b-112">Pentru a afla mai multe despre raportul de sincronizare de la AAD Connect Health și despre cum să îl descărcați, consultați [raportul de sincronizare la nivel de obiect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="ce93b-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="ce93b-113">Pentru a depana avertizările de sănătate din Dan Connect, urmați [Ghidul de depanare pentru depanarea alertelor de stare a stării de sănătate](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) și pentru întrebări frecvente, consultați [întrebări comune despre instalarea](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problemelor de sănătate.</span><span class="sxs-lookup"><span data-stu-id="ce93b-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
