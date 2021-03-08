---
title: Atribuirea unui rol de jurnal de audit în centrul de conformitate & securitate Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526527"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="5bc1b-102">Atribuirea unui rol de jurnal de audit în centrul de conformitate & securitate Office 365</span><span class="sxs-lookup"><span data-stu-id="5bc1b-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="5bc1b-103">Pentru a căuta în Jurnalul de auditare Office 365, unui administrator trebuie să i se atribuie rolul de **jurnal de audit doar pentru vizualizare** sau rolul **jurnalelor de auditare** în Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5bc1b-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="5bc1b-104">Aceste roluri sunt atribuite în mod implicit grupurilor de roluri pentru gestionarea conformității și gestionarea organizației.</span><span class="sxs-lookup"><span data-stu-id="5bc1b-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="5bc1b-105">Administratorii globali din Office 365 și Microsoft 365 sunt adăugați automat ca membri ai grupului de roluri Gestionare organizație.</span><span class="sxs-lookup"><span data-stu-id="5bc1b-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="5bc1b-106">Pentru a permite unui utilizator să caute cu nivelul minim de privilegii, creați un grup de roluri particularizat în Exchange Online, **Adăugați rolul de** jurnal de auditare pentru rolurile de **Audit doar pentru vizualizare** , apoi adăugați utilizatorul ca membru al grupului de roluri nou.</span><span class="sxs-lookup"><span data-stu-id="5bc1b-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="5bc1b-107">Pentru mai multe informații, consultați [gestionarea grupurilor de roluri în Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) și [căutarea în Jurnalul de auditare din centrul de conformitate & de securitate](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="5bc1b-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>