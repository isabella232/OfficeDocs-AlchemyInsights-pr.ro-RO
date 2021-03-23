---
title: Notificare Dan Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037239"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="ae4a8-102">Notificare Dan Connect</span><span class="sxs-lookup"><span data-stu-id="ae4a8-102">Notification AAD Connect</span></span>

- <span data-ttu-id="ae4a8-103">Asigurați-vă că sunteți autorizat să efectuați operațiunea.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="ae4a8-104">Administratorii globali au acces în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-104">Global Admins have access by default.</span></span> <span data-ttu-id="ae4a8-105">În plus, puteți utiliza [controlul Access bazat pe roluri](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) pentru a delega permisiunea de înregistrare la colaborator.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="ae4a8-106">Asigurați-vă că punctele finale necesare sunt activate și nu sunt blocate din cauza firewallului.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="ae4a8-107">Pentru detalii, consultați [cerințe](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="ae4a8-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="ae4a8-108">Înregistrarea poate să nu reușească din cauza comunicării de ieșire supusă inspecției SSL de către stratul de rețea.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="ae4a8-109">Asigurați-vă că ați verificat setările de notificare pentru Azure AD Connect Health și revizuiți setarea.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="ae4a8-110">Pentru a înțelege cum să configurați setările de notificare pentru notificările de sănătate Azure AD Connect, consultați acest [Ghid](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="ae4a8-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="ae4a8-111">Pentru a afla mai multe despre raportul de sincronizare de la AAD Connect Health și despre cum să îl descărcați, consultați [raportul de sincronizare la nivel de obiect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="ae4a8-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="ae4a8-112">Pentru a depana avertizările de sănătate din AAD Connect, urmați [Ghidul de depanare pentru depanarea alertelor de stare a stării](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) de bună funcționare a datelor și pentru întrebări frecvente, consultați [întrebări frecvente despre instalarea](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problemelor de sănătate.</span><span class="sxs-lookup"><span data-stu-id="ae4a8-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
