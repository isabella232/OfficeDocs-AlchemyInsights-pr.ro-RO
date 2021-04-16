---
title: Retransmisia e-mailului prin Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809667"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="00785-102">Configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite mesaje de e-mail</span><span class="sxs-lookup"><span data-stu-id="00785-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="00785-103">Pentru a afla opțiunile și pașii, consultați [Cum să configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite e-mail utilizând Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="00785-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="00785-104">**Notă:** dacă aveți un dispozitiv sau o aplicație care recent a încetat să funcționeze, vă rugăm să rețineți că am început recent [să dezactivăm cifrul 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption), conform planificării.</span><span class="sxs-lookup"><span data-stu-id="00785-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="00785-105">Pentru a vedea dispozitivele afectate, accesați [Raportul clienților cu autentificare SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="00785-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="00785-106">Erorile uzuale ar putea fi similare cu: Eroarea de autentificare, Eroarea TLS, Eroarea algoritmului de cifrare, Nepotrivirea de algoritm sau Conexiunea abandonată.</span><span class="sxs-lookup"><span data-stu-id="00785-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="00785-107">Pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="00785-107">To resolve the issue:</span></span>

 - <span data-ttu-id="00785-108">**Windows Server 2003 IIS SMTP nu va mai funcționa - este necesară o versiune mai nouă de Windows.**</span><span class="sxs-lookup"><span data-stu-id="00785-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="00785-109">Consultați furnizorul aplicației sau al dispozitivului pentru a vedea dacă este acceptat un cifru modern sau dacă există o actualizare.</span><span class="sxs-lookup"><span data-stu-id="00785-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
